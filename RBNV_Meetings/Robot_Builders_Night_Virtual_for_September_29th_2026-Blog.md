# When Yaw Goes Sideways: Debugging BNO Quaternions Across Python and C++

*Robot Builders Night Virtual — September 29, 2026*

Orientation math took center stage at this week’s Dallas Personal Robotics Group Robot Builders Night Virtual. The discussion focused on a familiar robotics challenge: converting quaternion output from a BNO orientation sensor into a dependable yaw angle.

Although the Python and C++ implementations looked nearly identical, the conversation demonstrated why quaternion bugs are rarely caused by `atan2()` alone. Component ordering, coordinate frames, axis definitions, rotation conventions, and unit conversions can all produce plausible-looking—but incorrect—headings.

The group also touched on spare-board planning and wrapped up with a robotics-oriented dart-gun project shared by Scott Horton.

## Comparing Quaternion-to-Yaw Formulas

Mark R shared part of a Python calculation for extracting yaw from a quaternion:

```python
siny_cosp = 2.0 * (quat_real * quat_k + quat_i * quat_j)
```

Mike Williamson supplied the corresponding C++ calculation:

```cpp
double yaw = std::atan2(
    2.0 * (real * k + i * j),
    1.0 - 2.0 * (j * j + k * k)
);
```

If the quaternion is represented as:

\[
q = (w, x, y, z)
\]

with `real = w`, `i = x`, `j = y`, and `k = z`, Mike’s code becomes:

\[
\text{yaw} =
\operatorname{atan2}
\left(
2(wz + xy),
1 - 2(y^2 + z^2)
\right)
\]

This is a commonly used expression for rotation about the Z axis under one widely used quaternion and Euler-angle convention. The result from `atan2()` is in radians and normally falls in the range \([-\pi,\pi]\).

In Python, an equivalent implementation would be:

```python
import math

def quaternion_to_yaw(w, x, y, z):
    siny_cosp = 2.0 * (w * z + x * y)
    cosy_cosp = 1.0 - 2.0 * (y * y + z * z)
    return math.atan2(siny_cosp, cosy_cosp)
```

For degrees:

```python
yaw_degrees = math.degrees(quaternion_to_yaw(w, x, y, z))
```

The important rule is to perform that conversion **once**.

## Similar Formulas May Describe Different Angles

Mark Dombrowski offered another expression:

```cpp
var yaw = atan2(
    2.0 * (q.y * q.z + q.w * q.x),
    q.w * q.w - q.x * q.x - q.y * q.y + q.z * q.z
);
```

For a normalized quaternion, the denominator is equivalent to:

\[
1 - 2(x^2 + y^2)
\]

Under the common \(w,x,y,z\) convention, this expression often corresponds to rotation around the **X axis**, commonly labeled roll—not Z-axis yaw.

That does not automatically make the formula wrong. It may indicate that the code uses:

- A different quaternion component order
- A different choice of “up” axis
- Intrinsic rather than extrinsic rotations
- Active rather than passive rotations
- A different handedness or coordinate frame
- Different meanings for roll, pitch, and yaw

Robotics systems frequently mix coordinate conventions. An IMU library, visualization package, vehicle controller, and mechanical drawing may each use different axis definitions. ROS, for example, standardizes coordinate-frame practices in [REP 103](https://www.ros.org/reps/rep-0103.html), but sensor APIs do not necessarily follow the same convention.

Before choosing a formula, developers should answer four questions:

1. In what order does the API return quaternion components?
2. Which physical axis should represent yaw?
3. What are the positive rotation direction and coordinate handedness?
4. In what order are Euler rotations applied?

## The Likely Culprit: Degrees Converted Twice

D Steele relayed an analysis from Claude that identified a likely unit bug: one line appeared to convert an angle to degrees twice.

Most standard trigonometric functions—including Python’s `math.atan2()` and C++’s `std::atan2()`—return radians. A single conversion is appropriate:

```python
yaw_deg = math.degrees(yaw_rad)
```

or:

```cpp
double yaw_deg = yaw_rad * 180.0 / std::numbers::pi;
```

Applying the factor \(180/\pi\) a second time multiplies the expected result by approximately 57.3. For example, a correct heading of 90 degrees could become roughly 5,157 degrees.

A good debugging practice is to keep radians and degrees in explicitly named variables:

```python
yaw_rad = math.atan2(siny_cosp, cosy_cosp)
yaw_deg = math.degrees(yaw_rad)
```

This makes accidental reconversion easier to spot.

## Better Debugging Through Named Values

Mike highlighted Python’s self-documenting f-string syntax:

```python
print(f"{var1=} {var2=}")
```

Introduced in Python 3.8, the `=` form prints both the expression and its value. It is especially useful when comparing intermediate orientation calculations:

```python
print(f"{w=} {x=} {y=} {z=}")
print(f"{siny_cosp=} {cosy_cosp=}")
print(f"{yaw_rad=} {yaw_deg=}")
```

Equivalent C++ output might look like:

```cpp
std::cout
    << "w=" << w
    << " x=" << x
    << " y=" << y
    << " z=" << z
    << " siny_cosp=" << siny_cosp
    << " cosy_cosp=" << cosy_cosp
    << " yaw_rad=" << yaw_rad
    << '\n';
```

Printing the same intermediate values in both languages is more useful than comparing only the final angle. It helps identify exactly where two implementations begin to diverge.

## A Practical Quaternion Debugging Checklist

For anyone facing a similar orientation problem, the meeting discussion suggests a systematic test process.

### 1. Verify component order

Do not assume the sensor returns \(w,x,y,z\). APIs may use:

- \(w,x,y,z\)
- \(x,y,z,w\)
- `real, i, j, k`
- A device-specific structure

Confirm the order in the documentation for the exact sensor and software library.

### 2. Check quaternion normalization

The common formulas generally assume a unit quaternion:

\[
w^2+x^2+y^2+z^2=1
\]

A simple diagnostic is:

```python
norm_sq = w*w + x*x + y*y + z*z
print(f"{norm_sq=}")
```

Small floating-point deviations are normal, but a value far from 1 may indicate corrupted data, scaling problems, or incorrect component parsing.

### 3. Test known orientations

Start with the identity quaternion:

```text
(w, x, y, z) = (1, 0, 0, 0)
```

The calculated yaw should be zero under the standard convention.

For a 90-degree rotation around Z:

```text
(w, x, y, z) ≈ (0.7071, 0, 0, 0.7071)
```

The expected yaw is approximately:

```text
1.5708 radians
90 degrees
```

Known test vectors are often more revealing than live sensor data.

### 4. Confirm the physical axis

Rotate the sensor around one axis at a time and observe which quaternion components and Euler angles change. Sensor mounting can make a mathematically correct Z-axis angle inappropriate for the robot’s physical definition of heading.

Some BNO devices and libraries support axis remapping, so both the mounting orientation and any software remapping should be documented.

### 5. Separate conversion from angle wrapping

`atan2()` generally returns angles from \(-\pi\) to \(+\pi\), or \(-180^\circ\) to \(+180^\circ\). Applications that require a compass-style range can wrap the result:

```python
yaw_deg_360 = yaw_deg % 360.0
```

Do this separately from quaternion conversion so that wrapping does not hide a deeper convention or unit error.

### 6. Consider calibration and fusion mode

A correct formula cannot compensate for an uncalibrated sensor or an unsuitable fusion mode. Absolute heading typically depends on magnetometer data, making it sensitive to nearby motors, steel hardware, wiring currents, and magnetic interference.

Developers using devices such as the BNO055 should consult the exact device and library documentation, including Bosch Sensortec’s [BNO055 product information](https://www.bosch-sensortec.com/products/smart-sensor-systems/bno055/) and Adafruit’s [BNO055 guide](https://learn.adafruit.com/adafruit-bno055-absolute-orientation-sensor).

## Hardware Planning: How Many Spares Are Enough?

Ed Mart asked Tom how many “CYD” boards he had purchased. In electronics circles, CYD commonly refers to the inexpensive ESP32-based **Cheap Yellow Display** boards, although the exact model was not specified in the available discussion.

The larger question was broadly applicable: how many spare controllers should a project keep on hand?

There is no universal answer, but practical factors include:

- Component lead time
- Probability of damage during wiring and prototyping
- Whether boards are needed for parallel development
- Differences between board revisions
- The cost of project downtime
- Whether firmware and wiring should be tested on an untouched reference unit

For low-cost development boards, a useful minimum is often:

1. One board installed in the robot
2. One board on the bench for firmware testing
3. One known-good spare

That is a planning guideline rather than a recommendation reached by the group. Higher-risk projects, public demonstrations, and boards with inconsistent availability may justify additional inventory.

## Project Spotlight: Scott Horton’s Dart Gun

Near the end of the meeting, Scott Horton shared his [`rshorton/dart_gun`](https://github.com/rshorton/dart_gun) GitHub repository.

The available meeting notes did not include a detailed walkthrough, but the repository offers builders a starting point for exploring the project directly. Automated dart launchers can bring together several robotics disciplines, including actuation, aiming, embedded control, sensing, and mechanical design.

As with any projectile mechanism, builders should prioritize safe testing procedures, positive firing interlocks, controlled test areas, and reliable power isolation during maintenance.

## Closing Thoughts

This week’s discussion illustrated a core lesson in robotics software: equations cannot be separated from their conventions.

Two quaternion formulas may both be mathematically valid while calculating different physical rotations. Likewise, matching Python and C++ code can still produce incorrect results if the quaternion components are mislabeled, the wrong axis is treated as yaw, or radians are converted to degrees twice.

The most effective debugging strategy is therefore layered:

- Confirm the sensor’s quaternion definition
- Verify the coordinate frame and desired axis
- Check normalization
- Test with known quaternions
- Print intermediate terms
- Convert units exactly once
- Validate the result against physical motion

With those checks in place, quaternion debugging becomes less mysterious—and much less likely to send a robot confidently in the wrong direction.

## Suggested Images and Diagrams

- A labeled quaternion diagram showing \(w,x,y,z\)
- A robot coordinate frame illustrating roll, pitch, and yaw
- A side-by-side Python and C++ conversion flowchart
- A graph comparing radians, degrees, and double-converted values
- A photo or architecture diagram from Scott Horton’s dart-gun repository, subject to its license and attribution requirements
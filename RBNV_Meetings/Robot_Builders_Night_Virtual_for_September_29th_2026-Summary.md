# Robot Builders Night Virtual for September 29th, 2026

## Introduction

The meeting focused on debugging orientation calculations from a BNO sensor, particularly converting quaternion data into yaw values in Python and C++. Participants also briefly discussed hardware purchasing and spare-board planning before Scott Horton shared a robotics-oriented dart-gun project repository.

## BNO Sensor Yaw and Quaternion Calculations

- Mark R shared a Python function for reading yaw from a BNO sensor and provided part of the quaternion conversion formula:
  ```python
  siny_cosp = 2.0 * (quat_real * quat_k + quat_i * quat_j)
  ```
- Mike Williamson shared the corresponding C++ yaw calculation:
  ```cpp
  double yaw = std::atan2(
      2.0 * (real * k + i * j),
      1.0 - 2.0 * (j * j + k * k)
  );
  ```
- Mark R noted that Mike’s C++ implementation was very similar to his Python version.
- Mark Dombrowski supplied an alternative quaternion-to-angle expression:
  ```cpp
  var yaw = atan2(
      2.0 * (q.y * q.z + q.w * q.x),
      q.w * q.w - q.x * q.x - q.y * q.y + q.z * q.z
  );
  ```
- The differing formulas appear to reflect quaternion component conventions, axis selection, or rotation-order assumptions. These details should be verified against the sensor library’s definitions.
- D Steele relayed an analysis from Claude and identified a likely bug: one line was converting an angle to degrees twice.
- Mike also highlighted Python’s convenient debug-printing syntax:
  ```python
  print(f"{var1=} {var2=}")
  ```
  This can make it easier to inspect intermediate quaternion and angle values.

## Hardware Purchasing and Spare Planning

- Ed Mart asked Tom how many “CYD” boards he purchased.
- The group also raised the practical question of how many spare units should be kept on hand to provide confidence during development.
- No final quantity or purchasing recommendation was captured in the supplied conversation.

## Dart-Gun Robotics Project

- Scott Horton shared the [`dart_gun`](https://github.com/rshorton/dart_gun) GitHub repository near the end of the meeting.
- The repository was presented as a relevant project resource, although no detailed technical discussion about its design or operation was included in the available chat.

# Conclusions and Insights

- Most of the technical discussion centered on validating quaternion-to-yaw conversion code across Python and C++.
- The implementations are structurally similar, but developers should confirm:
  - Quaternion component ordering and naming
  - Which axis is being treated as yaw
  - Rotation conventions and coordinate systems
  - Whether the result is in radians or degrees
- The suspected double conversion to degrees is an important debugging finding and may explain incorrect angle output.
- Printing named intermediate values can help compare implementations and isolate mathematical or unit-conversion errors.
- Hardware projects should account for spare controllers or boards, though the group did not establish a specific recommended quantity.

## Referenced Links by Contributor

### Scott Horton

- [rshorton/dart_gun](https://github.com/rshorton/dart_gun) — GitHub repository for the dart-gun project shared during the meeting.
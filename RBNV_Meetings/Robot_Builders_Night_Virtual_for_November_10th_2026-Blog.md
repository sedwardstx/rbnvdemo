# From Printable Wheels to Waddling Robots: Highlights from DPRG’s November 10 Robot Builders Night

The November 10, 2026 edition of the Dallas Personal Robotics Group’s Robot Builders Night Virtual moved across three very different—but surprisingly connected—areas of robot building: parametric CAD, characterful locomotion, and immersive project documentation.

A proposed demonstration of a Fusion-based wheel generator showed how small design tools can accelerate mechanical development. A conversation about robotic ducks explored the challenges of making machines move with personality. Finally, the group considered how 360-degree cameras can improve the way dynamic robots and motorsports projects are recorded.

## Generating Printable Robot Wheels in Autodesk Fusion

At **01:02:11**, Karim Virani asked how many participants use [Autodesk Fusion](https://www.autodesk.com/products/fusion-360/overview) for computer-aided design. Pat Caron responded by suggesting that Karim give a demonstration of his printable wheel generator.

Karim explained that the generator is currently specific to Fusion and, mindful of the meeting schedule, kept the discussion brief. Nevertheless, the exchange revealed interest in a subject that could easily support a future technical presentation.

### Why a wheel generator is useful

Robot wheels may look simple, but they often need to satisfy several project-specific constraints:

- Wheel diameter and width
- Axle bore or hub dimensions
- Motor-shaft interfaces
- Tire or tread geometry
- Clearance around motors and chassis components
- Printer tolerances and material properties

A parametric generator can turn those dimensions into editable inputs rather than requiring builders to remodel a wheel from scratch. That becomes especially valuable when a robot goes through several design revisions or when a builder needs a family of wheels for different motors and surfaces.

Fusion is well suited to this workflow because its parametric modeling tools allow dimensions and relationships to drive the final geometry. A future demonstration could cover not only how the generator works, but also practical fabrication questions such as bore compensation, tread selection, layer orientation, and the choice between rigid filament and flexible materials such as TPU.

### Opportunities beyond Fusion

The conversation also raised an implicit portability question. If the generator proves useful, builders who prefer FreeCAD, OpenSCAD, Onshape, or another CAD environment may want access to the same capabilities.

Potential paths toward broader support could include:

1. Exporting generated wheels as STEP or STL files.
2. Publishing a documented set of design parameters.
3. Reimplementing the design in script-based CAD.
4. Separating the wheel-generation mathematics from Fusion-specific automation.

No such expansion was announced during the meeting, but it would make an interesting topic for future collaboration.

## When a Waddle Becomes a Robotics Problem

Ed Mart’s mention of the **XGo duck** shifted the conversation from wheels to legs—and from purely functional machines to robots designed around recognizable character and motion.

Tom Crawford added an article from *Make:* about [OpenDuck/OpenBDX learning to waddle](https://makezine.com/article/technology/robotics/openbdx-duck-robot-learning-to-waddle/). Mark Dombrowski also shared a [YouTube video](https://www.youtube.com/watch?v=DoY3duDDiUA) during the discussion.

Duck-inspired robots are entertaining, but their movement presents serious engineering challenges. A convincing waddle involves more than alternately moving two legs. The controller must manage balance, weight transfer, foot placement, body orientation, and recovery from small disturbances.

### Why expressive locomotion matters

Traditional mobile robots are often judged by speed, accuracy, or payload. Character robots add another requirement: their motion must communicate personality.

That changes the design problem. A motion can be mechanically successful yet visually unconvincing. Conversely, a slightly exaggerated gait may appear more natural or expressive to a human observer, even if it is not the most energy-efficient way to move.

Projects such as OpenDuck/OpenBDX demonstrate the growing overlap among:

- Mechanical design and 3D printing
- Servo selection and actuator control
- Inertial sensing and balance estimation
- Gait generation
- Simulation and learning-based control
- Animation principles and human-robot interaction

The waddling motion is therefore more than a novelty. It is a compact example of embodied robotics, in which the robot’s physical form, controller, and perceived personality all influence one another.

### Simulation-to-reality remains the hard part

Learning a gait in simulation can reduce the risk and cost of physical testing, but a simulated robot never matches hardware perfectly. Real joints have backlash, printed parts flex, batteries change mass distribution, servos heat up, and feet interact unpredictably with different surfaces.

Successful transfer to a physical robot typically requires careful modeling, conservative testing, and control strategies that tolerate uncertainty. For hobby and research platforms alike, the most revealing moment is often not when a robot walks in simulation, but when it takes its first stable steps on an actual floor.

## Capturing Robots with 360-Degree Cameras

The evening’s third major topic concerned how projects are recorded. Ed Mart observed that [Insta360](https://www.insta360.com/) cameras have become popular in motorsports, where fast motion and unpredictable action make conventional framing difficult.

The same benefits apply to mobile robots.

Most consumer 360-degree cameras use lenses on opposite sides of the camera to capture nearly the entire surrounding scene. Software stitches those views together, allowing the operator to select a conventional camera angle later. Instead of perfectly tracking a moving robot during filming, a builder can concentrate on the test and reframe the footage afterward.

### Robotics applications

A 360-degree camera could be particularly helpful for:

- Outdoor rover trials
- Robot races and competitions
- Autonomous navigation tests
- Walking-robot demonstrations
- Chassis-mounted point-of-view footage
- Workshop and event documentation
- Recording interactions among several robots

Image stabilization can also improve footage from vibrating or rapidly moving platforms. Pole-mounted cameras may produce an elevated chase-camera perspective, while some systems can visually minimize a compatible selfie stick in the stitched image.

### Practical limitations

These cameras are not a universal replacement for conventional video equipment. Builders should account for:

- Distortion and stitching artifacts near lens boundaries
- Reduced detail after reframing a small part of the full image
- Vulnerable protruding lenses
- Large files and additional editing requirements
- Low-light performance
- Vibration at the camera mount
- The effect of camera weight on a small robot’s balance

For technical documentation, a 360-degree view is often most effective when paired with conventional close-ups, onboard telemetry, and fixed wide-angle footage.

## Three Tools, One Iterative Workflow

Although printable wheels, waddling ducks, and motorsports cameras initially seem unrelated, they represent three stages of the same engineering cycle:

1. **Design the mechanism** with reusable CAD tools.
2. **Develop and test the behavior** on real hardware.
3. **Record the results** clearly enough to evaluate and share them.

Karim’s wheel generator could shorten the first stage. Duck-inspired platforms demonstrate the complexity of the second. A 360-degree camera can strengthen the third by capturing details that might otherwise be missed during a fast or unpredictable test.

That full loop matters to community robotics. Good documentation helps builders diagnose failures, compare revisions, teach others, and turn a one-off experiment into a reproducible project.

## Looking Ahead

Karim Virani’s Fusion wheel generator appears to be a strong candidate for a future Robot Builders Night demonstration. A focused session could explore the generator’s parameter set, printing considerations, and whether its underlying approach could be adapted for other CAD platforms.

The robotic-duck discussion also points toward a broader trend: robots are increasingly expected not merely to move, but to move expressively. Open platforms such as OpenDuck/OpenBDX make those experiments more accessible to independent builders.

Meanwhile, 360-degree cameras offer a practical way to document those machines in motion. As robotics projects become faster, more mobile, and more visually engaging, the tools used to record them are becoming part of the engineering workflow itself.

## Suggested Visuals

- A screenshot of Karim Virani’s wheel generator showing its editable Fusion parameters
- A diagram comparing wheel diameter, hub, axle bore, and tread dimensions
- An image or animation of OpenDuck/OpenBDX during a walking test
- A gait diagram illustrating side-to-side weight transfer during a waddle
- A diagram showing how a dual-lens 360-degree camera captures and stitches a spherical view
- A comparison between raw 360-degree footage and a reframed robot-tracking shot

## References

- [Autodesk Fusion](https://www.autodesk.com/products/fusion-360/overview)
- [OpenBDX Duck Robot Learning to Waddle — *Make:*](https://makezine.com/article/technology/robotics/openbdx-duck-robot-learning-to-waddle/)
- [Video shared by Mark Dombrowski](https://www.youtube.com/watch?v=DoY3duDDiUA)
- [Insta360](https://www.insta360.com/)
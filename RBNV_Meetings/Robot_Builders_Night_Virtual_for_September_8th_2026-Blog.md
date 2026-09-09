# Open-Source Robots, Unconventional Locomotion, and the Glow of Tritium

*Robot Builders Night Virtual — September 8, 2026*

The September 8 Robot Builders Night Virtual meeting highlighted one of the strongest ideas in hobby robotics: a project becomes far more valuable when other builders can inspect it, reproduce it, and improve it.

Links shared during the meeting ranged from snake-inspired machines and compact desktop robots to tritium illumination components. The discussion also touched on *Smarter Every Day*, connecting hands-on robot building with the broader world of science and engineering education.

Because no voice transcript was available, this recap is based on the meeting chat and its shared resources.

## Three Paths into Open-Source Robotics

Pat Caron contributed three projects that offer different entry points into open-source robot development:

- [SnakeROS](https://github.com/kevinmcaleer/SnakeROS)
- [SKD1](https://github.com/gmsanchez/skd1)
- [Petoi Quaddle](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit)

Collectively, these projects point toward an important trend: small robots are becoming capable platforms for exploring locomotion, embedded control, software architecture, and mechanical design without requiring an industrial-scale budget.

## SnakeROS: Coordinating a Robot with Many Joints

[SnakeROS](https://github.com/kevinmcaleer/SnakeROS), shared at approximately 00:17:46, explores snake-style robotics through an openly available repository.

Snake robots present an unusual control problem. A conventional differential-drive robot may have only two primary wheel commands, while an articulated snake must coordinate a chain of joints. Useful motion emerges from the phase, amplitude, and offset relationships among those joints.

A simplified traveling-wave command can be expressed as:

\[
\theta_i(t)=A\sin(\omega t+i\phi)+b
\]

where:

- \(\theta_i\) is the target angle for joint \(i\)
- \(A\) controls bending amplitude
- \(\omega\) determines oscillation speed
- \(\phi\) sets the phase difference between adjacent joints
- \(b\) provides a steering or posture offset

That equation is only a starting point. Real hardware introduces servo limits, backlash, uneven friction, power constraints, and timing jitter. Even so, a wave-based controller gives builders a manageable way to experiment with gaits and turning behavior.

The project name also underscores the value of organizing robot capabilities through the [Robot Operating System](https://www.ros.org/). ROS and [ROS 2](https://docs.ros.org/) encourage developers to divide a robot into components for actuation, sensing, visualization, control, and higher-level behavior. That modularity is especially useful for a multi-jointed platform.

### Why Snake Robots Matter

Snake-inspired machines can potentially navigate places that are difficult for wheeled or legged robots, including:

- Pipes and confined passages
- Rubble and inspection spaces
- Uneven terrain
- Areas where a low profile is advantageous

For hobbyists, they are also excellent laboratories for learning about synchronized motion, gait generation, distributed actuation, and the difference between simulated movement and physical performance.

## SKD1: A Repository Worth Studying, Not Just Running

The second repository, [SKD1](https://github.com/gmsanchez/skd1), was shared at approximately 00:19:03.

Open-source robot repositories are useful even when a builder does not intend to reproduce the complete machine. They can reveal how another designer divided the system into mechanical, electrical, and software layers.

When evaluating SKD1—or any community robotics project—it is worth looking for:

1. **Mechanical design files**  
   Are CAD models, printable parts, and assembly guidance available?

2. **Electronics documentation**  
   Does the project provide wiring diagrams, pin assignments, and power requirements?

3. **Software structure**  
   Is the code separated into hardware drivers, motion control, and behaviors?

4. **Bill of materials**  
   Are the specified components still obtainable, and are alternatives documented?

5. **License information**  
   “Open source” is most useful when the permissions for code, hardware, and documentation are clearly stated.

6. **Reproducibility notes**  
   Does the repository explain calibration, configuration, and known limitations?

This kind of review turns a GitHub repository into an engineering lesson. A project’s most valuable contribution may not be its finished robot, but rather a reusable mechanism, control method, enclosure technique, or software pattern.

## Petoi Quaddle: Open Robotics on the Desktop

At approximately 00:24:49, Pat shared the Kickstarter page for [Petoi Quaddle](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit), presented as an open-source desktop robot kit.

Desktop robots occupy a productive middle ground. They are small enough to operate safely in a home, classroom, or makerspace, yet capable enough to demonstrate:

- Multi-servo coordination
- Legged locomotion
- Balance and posture control
- Sensor integration
- Programmable behaviors
- Mechanical calibration

Petoi is also associated with the open-source [OpenCat](https://github.com/PetoiCamp/OpenCat) quadruped framework, which supports programmable robotic pets and educational experimentation. Platforms in this category lower the barrier to studying legged motion because builders can begin with an assembled or kit-based mechanism rather than designing every linkage from scratch.

### “Open Source” Has Several Layers

For robot kits, openness is rarely a single yes-or-no property. Builders should consider whether a platform provides access to:

- Application code
- Low-level motion firmware
- Communication protocols
- Mechanical design files
- Electronics schematics
- Calibration tools
- Modification and redistribution rights

A robot with programmable behaviors is useful, but a robot with documented hardware and modifiable control software is much more valuable as an engineering platform.

Crowdfunding projects carry additional considerations. Specifications, schedules, pricing, and deliverables may change during development, so prospective backers should consult the campaign’s current documentation before making decisions.

## Comparing the Three Projects

The projects shared during the meeting illustrate complementary approaches to robotics:

| Project | Primary value for builders | Likely learning focus |
|---|---|---|
| [SnakeROS](https://github.com/kevinmcaleer/SnakeROS) | Articulated, unconventional locomotion | Joint coordination, gait generation, ROS-based organization |
| [SKD1](https://github.com/gmsanchez/skd1) | Open repository for design study and experimentation | System architecture, fabrication, electronics, software reuse |
| [Petoi Quaddle](https://www.kickstarter.com/projects/petoi/quaddle-open-source-desktop-robot-kit) | Compact kit-oriented robotics platform | Legged motion, calibration, programming, educational robotics |

They also demonstrate three ways to engage with open-source hardware:

- Build a project as documented.
- Extract one subsystem for use elsewhere.
- Study the design and create a different implementation.

That third option is often overlooked. Open projects are not merely kits to copy; they are engineering references.

## Tritium Vials: Light Without Wires or Batteries

Later in the meeting, at approximately 01:10:28, Ponder SomeMore shared the [Tritium Workshop collection of tritium vials](https://tritiumworkshop.com/collections/tritium-vials).

Tritium is a radioactive isotope of hydrogen. In a tritium light source, a small quantity of gas is sealed inside a vial whose interior has a phosphor coating. Low-energy beta emissions stimulate the phosphor, producing a continuous glow without an external power supply.

With a half-life of approximately 12.3 years, tritium can provide long-duration illumination, although its brightness gradually decreases over time.

Potential maker applications include:

- Passive location markers
- Low-light orientation indicators
- Props and display pieces
- Markers that must remain visible without wiring
- Decorative accents

For most robots, LEDs remain the more practical choice. They are brighter, controllable, inexpensive, and available in many packages. Tritium’s advantages are that it requires no wiring and continues glowing when the robot is completely unpowered.

### Safety and Legal Considerations

Tritium vials should be treated as sealed, specialized products—not as components to cut, drill, open, or modify. Damaged vials require appropriate handling, and rules concerning sale, possession, importation, shipping, and disposal vary by jurisdiction.

Builders should purchase only from reputable suppliers, verify local regulations, and follow the manufacturer’s handling instructions. A passive glow is interesting, but it does not justify unsafe fabrication practices.

## Smarter Every Day and the Importance of Engineering Communication

Near 01:30:26, the chat mentioned Destin Sandlin and [Smarter Every Day](https://www.smartereveryday.com/), although no specific episode was identified.

The reference fits naturally with Robot Builders Night. Destin’s work frequently uses high-speed imaging, experiments, and interviews to make complicated physical systems understandable. That approach offers a useful lesson for robot builders: document not only whether a machine works, but also *why* it behaves as it does.

For robotics projects, effective documentation might include:

- Slow-motion footage of a mechanism
- Current measurements during startup and stall
- Joint-position plots
- Gait diagrams
- Failure analysis
- Comparisons between simulated and physical motion
- Clear explanations of design tradeoffs

A well-documented failure can teach the community more than an unexplained success.

## Final Thoughts

The September 8 meeting chat offered a compact tour of the modern maker ecosystem. SnakeROS introduced the challenge of coordinated articulated motion. SKD1 provided another open repository to examine and learn from. Petoi Quaddle highlighted the growing accessibility of desktop legged robots. Tritium vials expanded the conversation into unusual passive components, while the mention of *Smarter Every Day* emphasized the importance of curiosity and clear engineering communication.

The common thread is access: access to designs, source code, specialized parts, and understandable technical knowledge. Open-source robotics works best when projects move beyond demonstrations and provide enough information for others to reproduce results, diagnose problems, and create something new.

## Suggested Images and Diagrams

1. **Header collage:** A snake robot, a desktop legged robot, and a glowing tritium vial.
2. **Snake gait diagram:** A sequence showing phase-shifted joint angles along an articulated body.
3. **Open-robotics stack:** Mechanical design → electronics → firmware → middleware → behaviors.
4. **Project comparison graphic:** SnakeROS, SKD1, and Quaddle arranged by locomotion and learning focus.
5. **Tritium-vial cutaway:** A labeled conceptual diagram showing the sealed gas, phosphor coating, and emitted light.
6. **Repository evaluation checklist:** A visual summary covering CAD, schematics, code, bill of materials, documentation, and licensing.

> **Image note:** Use repository or campaign images only in accordance with their respective licenses and media permissions.
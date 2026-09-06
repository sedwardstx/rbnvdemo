# DPRG Sets Its 2026 Robotics Agenda: RoboRama, Remote Competition, ROS 2, AI, and the Return of Robie

The Dallas Personal Robotics Group opened its 2026 program year by looking backward—and then quickly turning toward what comes next.

During the January 24 Robot Builders Night Virtual meeting, DPRG members reviewed a busy 2025, unanimously elected a new leadership team, began refining the rules for RoboRama 2026, and proposed a practical technical program spanning ROS 2, artificial intelligence, communication buses, modular electronics, and structural 3D printing.

One theme connected nearly every discussion: converting the club’s accumulated knowledge into shared, repeatable work. That includes establishing equivalent contest courses for remote competitors, organizing project-focused builder nights, restoring the club’s full-size robot Robie, and making years of technical material easier to find online.

## A Strong Foundation from 2025

Outgoing president Paul Bouchier’s recorded annual review highlighted the breadth of DPRG’s activities during 2025.

The club held approximately 50 Robot Builders Night Virtual sessions, typically drawing 12 to 20 participants. Monthly meetings at the Dallas Makerspace continued to include remote attendees, while quarterly Robot Power Lunch gatherings provided another opportunity for informal collaboration.

Technical presentations covered a broad range of modern robot-building skills:

- PCB design using KiCad.
- ROS 2 navigation and Linorobot 2.
- Git and GitHub workflows.
- Voice-controlled robots connected to cloud-hosted large language models.
- AI-assisted video production.

DPRG also maintained a strong competition and outreach schedule. The club held its indoor RoboRama contests in May and participated in the outdoor RoboColumbus competition in November. Scott earned full marks on his first RoboColumbus run—an achievement that prompted interest in a future technical review of his robot’s mechanical, electronic, and software design.

Other activities included a RobotLAB visit, outreach to robotics groups at the University of Texas at Dallas and the University of Texas at Arlington, practice interviews for a student VEX team, and public demonstrations at Dallas Love Field.

The club ended the year with approximately 34 to 35 paid members. It also continued using AI-generated transcripts, summaries, and video chapters to make its frequent online meetings more accessible.

## DPRG Elects an International Board

The proposed 2026 officer slate was approved unanimously:

- **President:** Mark Reynolds  
- **Vice President:** Paul Bouchier  
- **Secretary:** Doug Paradis  
- **Treasurer:** Steve Edwards  
- **IT Officer:** Pat Caron  

Ron Grant reported 15 verified votes, including proxies. That represented about 43% of the membership and exceeded the required quorum.

Pat Caron’s participation gives the board an international dimension: he is based in Espanola, Ontario, Canada. That geographic reach is especially relevant as DPRG works to make remote competition a more integrated part of RoboRama.

## RoboRama 2026 Takes Shape

The club confirmed that its indoor RoboRama competition will return in May. The preliminary event list includes:

- Six Can.
- Quick Trip.
- Four Squares.
- Barrel Racing.
- Mini Sumo.
- Advanced Line Following.
- Search and Retrieval, if there is sufficient competitor interest.

“There and Back” was also discussed as an approachable contest for first-time builders. Entry-level events play an important role in robotics clubs because they give newcomers a constrained engineering problem without requiring an advanced perception or navigation stack.

### Line Following Remains a Core Challenge

Line following may appear simple, but advanced courses quickly expose weaknesses in sensing, control-loop tuning, mechanical alignment, and speed management.

Mark Reynolds plans to defend his previous line-following victory in the advanced event. Mike Williamson is considering converting a second mini-sumo robot into a line follower—an interesting reuse of a compact differential-drive platform.

DPRG’s Challenge course remains an especially difficult target. It has reportedly been completed in simulation, but not yet successfully on the physical course. That gap illustrates a familiar robotics problem: a controller that works in a clean simulation may still struggle with lighting variations, wheel slip, sensor noise, uneven floors, print imperfections, and imperfect actuator response.

Course files and contest resources are available in the club’s [DPRG Line Following Contest repository](https://github.com/dprg/Contests/tree/master/Line%20Following).

## Defining What Counts as a Competitive Run

Several proposed rule changes focused on ensuring that awards recognize meaningful robot performance.

One suggestion would require every robot to pass a minimum performance threshold before qualifying for a prize. For example:

- A line follower might have to navigate at least the first curve.
- A Six Can robot might have to place at least one can successfully.

The group also considered ways to handle multiple robots entered by the same builder. Options included limiting each person to two robots per event or allowing unlimited entries while restricting each competitor to one prize in that event.

Another proposal would require at least two entrants before an event counts as a competition. A sole entrant could still demonstrate the robot and receive recognition equivalent to third place, but would not automatically receive a first-place award.

These rules have not been finalized. However, they point toward a useful distinction between **participation**, **successful task execution**, and **competitive ranking**. Clear definitions in each category can make contests more welcoming to beginners while preserving the value of the awards.

Members also discussed a possible obstacle-avoidance event using an array of upright barriers. Such a contest could support several technical approaches, from simple bump sensors and ultrasonic ranging to lidar-based mapping and local path planning.

## Remote Competition Moves Toward Direct Competition

DPRG intends to continue supporting remote RoboRama participation. Pat Caron plans to explore hosting competitors at a recreation center in Espanola and promoting the event locally.

Importantly, Pat favored having remote robots compete directly against Dallas robots rather than receiving a separate, uncontested remote award.

Line following is particularly well suited to this model. Identical course artwork can be produced at multiple locations, allowing robots to run locally while their times and penalties are added to a shared ranking. DPRG is considering whether shipping a completed printed course from the United States would be less expensive and more consistent than having the course manufactured separately in Canada. [StickersBanners.com](https://stickersbanners.com/) was mentioned as a possible source for vinyl course printing.

Distributed competition still requires careful standardization. Organizers will need to control or document factors such as:

- Printed dimensions and scale.
- Surface finish and reflectivity.
- Line width and contrast.
- Course alignment.
- Timing procedures.
- Starting position and robot setup.
- Video evidence and judging standards.

A printed calibration ruler or known reference dimension on the course artwork could help remote organizers verify that a printer has not automatically resized the design.

## Combat Robots and Mini Sumo at UTD

Members also discussed attending a UTD Comet Robotics event scheduled for **Saturday, March 14, 2026**.

The event is expected to feature one-pound plastic, one-pound, and three-pound combat robots. Mini-sumo activity may also be available, giving Mike Williamson and other DPRG builders an opportunity to test their robots outside the regular RoboRama schedule.

Participants noted that SPARC-related competition rules may support or encourage partially autonomous combat robots. Autonomy adds an unusual engineering dimension to combat robotics: a machine must not only survive impacts but also detect, track, and approach an opponent within a rapidly changing arena.

## A Practical Technical Program for 2026

The proposed presentation schedule strongly emphasizes reusable engineering skills rather than one-off demonstrations.

### Mod Linker and Modular Electronics

Mark Dombrowski volunteered to present **Mod Linker**, or “module linker,” after the project is further developed.

The concept is intended to simplify communication between robot modules and potentially make modular electronic designs easier to build and share. A successful modular system must address more than connector shape. It may also need conventions for power distribution, signal voltage, addressing, message formats, mechanical mounting, and fault handling.

### Moving Beyond GPIO

A proposed introductory presentation would compare four common communication interfaces:

- **I²C**, often used for short-distance connections to low-speed sensors and peripherals.
- **SPI**, useful when higher speed and predictable timing are needed.
- **UART**, a simple and widely supported point-to-point serial interface.
- **CAN bus**, designed for robust multi-node communication and widely used in vehicles and industrial systems.

Understanding these interfaces is an important step beyond direct GPIO control. It allows builders to integrate smarter sensors, motor controllers, displays, distributed processors, and custom circuit boards.

### ROS 2 Without the Setup Overload

Members proposed a deliberately approachable ROS 2 presentation focused on establishing basic communication among a PC, Raspberry Pi, or microcontroller.

Workspace organization would be an important part of the discussion. A typical ROS 2 workspace produces `build`, `install`, and `log` directories in addition to the source tree. Generated files generally should not be committed to Git; the project’s source, launch files, maps, configuration, and documentation should be organized intentionally and protected with an appropriate `.gitignore`.

The group also wants to compare native and container-based development. Mike Williamson may demonstrate his non-Docker workflow, while Paul Bouchier may contribute guidance on Docker and GitHub practices.

Useful starting points include the official [ROS 2 documentation](https://docs.ros.org/en/rolling/index.html), [ROS 2 workspace tutorial](https://docs.ros.org/en/rolling/Tutorials/Beginner-Client-Libraries/Creating-A-Workspace/Creating-A-Workspace.html), and [Docker documentation](https://docs.docker.com/).

### AI Beyond “Vibe Coding”

At least two AI-oriented sessions were proposed.

The first would examine how builders can move beyond informal “vibe coding” toward disciplined use of coding agents. An AI assistant may produce working code quickly, but robotics software still requires:

- Explicit hardware and timing requirements.
- Version control.
- Repeatable tests.
- Interface definitions.
- Logging and diagnostics.
- Human review of safety-critical behavior.

The second presentation would compare local and cloud AI for robot perception. Cloud systems can offer powerful models, but they introduce network latency, service availability, recurring cost, and privacy concerns. Local inference can provide predictable operation without an internet connection, although it must fit within the robot’s processing, memory, power, and thermal limits.

Potential applications include object detection, computer vision, and a future search or retrieval competition. [OpenCV](https://opencv.org/) provides a broad foundation for image processing, while compact edge models can support detection and classification on Raspberry Pi-class computers and other embedded platforms.

### Designing Robot Parts for 3D Printing

Mark Dombrowski also offered to prepare a CAD-platform-independent talk on structural design for additive manufacturing.

Topics could include:

- Choosing print orientation based on expected loads.
- Designing around layer-direction weakness.
- Applying realistic fits, clearances, and tolerances.
- Creating assemblies that need little or no support material.
- Using heat-set threaded inserts.
- Selecting materials based on temperature, stiffness, toughness, and creep.
- Recognizing the limitations of PLA.
- Designing linear rails, joints, and other mechanisms.

Although Mark uses Fusion 360, these principles also apply to Onshape and other CAD systems. The emphasis would be on designing parts that function reliably, not merely parts that can be printed.

## Builder Nights with a Shared Mission

President Mark Reynolds proposed restarting regular in-person Robot Builders Night Out sessions, either weekly or every other week.

Rather than having each participant bring an unrelated project, the group favored organizing the meetings around a shared objective. This approach would allow tools, materials, test fixtures, and partially completed assemblies to remain ready between sessions. Work could be divided into clear mechanical, electrical, and software tasks.

Defined module interfaces would also let remote members contribute code or hardware without being physically present.

## Bringing Robie Back to Life

The leading candidate for the shared project is **Robie**, DPRG’s full-size club robot.

Potential upgrades include:

- Completing or redesigning the second arm.
- Detecting blocked or stalled joints.
- Improving mechanical and electrical safety.
- Adding modern vision capabilities.
- Adding speech output or voice recognition.
- Improving reliability for public demonstrations.
- Defining self-contained modules for remote contributors.

For safe operation around the public, blocked-joint detection could combine motor-current monitoring, position feedback, motion timeouts, and conservative force or torque limits. Physical emergency-stop controls and clearly defined operating modes would also be important.

Members favored completing the existing Robie before beginning a smaller successor. The robot’s large size makes it a strong visual attraction at events such as Moon Day.

A separate roaming robot could eventually travel through a venue, invite visitors to the DPRG display, and use supervised navigation to avoid people and obstacles. Such a platform would be an excellent integration project for mapping, human-aware navigation, speech, and remote oversight.

## Turning Club Knowledge into Documentation

DPRG would also like to publish more tutorials and project articles. The latest tutorial prominently visible on the club website reportedly dates to around 2022, despite years of technical discussions and working projects.

AI-assisted documentation could reduce the effort required to transform meeting notes, transcripts, source code, and design decisions into useful articles. Human technical review would remain essential, but AI could help produce first drafts, extract steps, organize troubleshooting notes, and create searchable summaries.

The club is also considering retrospective transcription and summarization of older Robot Builders Night Virtual recordings. Those videos contain valuable information, but much of it is difficult to discover without transcripts, chapters, tags, or written summaries.

Website performance is another concern. DPRG may need to request more resources from its current host or consider paid hosting to improve responsiveness and make an expanded technical archive practical.

## Building Toward a More Modular and Accessible Year

DPRG enters 2026 with stable membership, experienced leadership, and a full slate of possible projects. The club’s plans extend beyond simply holding more meetings or contests. They emphasize making robotics activities measurable, repeatable, shareable, and accessible across geographic boundaries.

RoboRama’s proposed minimum-performance rules could strengthen the meaning of competitive awards. Standardized printable courses could place Canadian and Texas robots in the same standings. Focused technical talks could help newcomers move from GPIO experiments to distributed systems, ROS 2, and edge AI. Most visibly, a collaborative restoration of Robie could unite those skills in one public-facing machine.

If DPRG succeeds in pairing that hands-on work with better tutorials, transcripts, and project documentation, its 2026 program will create more than robots—it will create a technical record that future builders can reuse.

## Suggested Images and Diagrams

1. **DPRG 2026 roadmap graphic** showing competitions, presentations, builder nights, and outreach activities.
2. **Line-following course photo or repository rendering**, with a robot positioned at the starting line.
3. **Remote competition diagram** connecting equivalent courses in Dallas and Espanola.
4. **Robot communications comparison chart** covering I²C, SPI, UART, and CAN bus.
5. **ROS 2 workspace diagram** showing source, build, install, log, configuration, and Git-tracked content.
6. **Robie before-restoration photograph**, annotated with proposed arm, vision, speech, and safety upgrades.
7. **3D-print orientation illustration** showing how layer direction affects the strength of a robot bracket.

## Resources

- [DPRG Line Following Contest Repository](https://github.com/dprg/Contests/tree/master/Line%20Following)
- [StickersBanners.com](https://stickersbanners.com/)
- [ROS 2 Documentation](https://docs.ros.org/en/rolling/index.html)
- [ROS 2: Creating a Workspace](https://docs.ros.org/en/rolling/Tutorials/Beginner-Client-Libraries/Creating-A-Workspace/Creating-A-Workspace.html)
- [Docker Documentation](https://docs.docker.com/)
- [OpenCV](https://opencv.org/)
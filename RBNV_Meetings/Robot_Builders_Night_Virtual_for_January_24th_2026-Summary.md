# Robot Builders Night Virtual for January 24th, 2026

## Introduction

The Dallas Personal Robotics Group (DPRG) opened its 2026 program with a review of the club’s 2025 activities, election of officers, and brainstorming for the coming year. Participants discussed RoboRama contests and rules, potential technical presentations, remote competition, project-focused builder nights, restoration of the club robot Robie, and improvements to DPRG’s website and technical documentation.

## 2025 Presidential Review

Outgoing president Paul Bouchier provided a recorded review of DPRG’s 2025 activities. Highlights included:

- Continued monthly in-person meetings at the Dallas Makerspace with remote participation.
- Quarterly Robot Power Lunch gatherings.
- Approximately 50 weekly Robot Builders Night Virtual meetings, generally attracting 12–20 participants.
- Continued use of AI-generated transcripts, meeting summaries, and video chaptering.
- Technical presentations covering:
  - KiCad PCB design.
  - ROS 2 navigation and Linorobot 2.
  - Git and GitHub.
  - Voice-controlled robots and cloud-based LLM interaction.
  - AI-generated video production.
- Competitions and events:
  - RoboRama indoor contests in May.
  - RoboColumbus outdoor competition in November, where Scott achieved full marks on his first run.
  - A visit to RobotLAB.
  - Outreach to UTD and UTA robotics groups.
  - Support for a student VEX team through practice interviews.
  - Public robot demonstrations at Dallas Love Field.
- Infrastructure improvements:
  - Continued use of Google Groups and Discord.
  - Regular website and YouTube updates.
  - Closure of the club’s Meetup.com subscription because its cost did not justify the results.
- DPRG ended the year with approximately 34–35 paid members.

Paul thanked the board, members, website volunteers, meeting organizers, and everyone supporting DPRG’s technical and outreach activities.

## 2026 Officer Election

The officer slate was approved unanimously.

- **President:** Mark Reynolds
- **Vice President:** Paul Bouchier
- **Secretary:** Doug Paradis
- **Treasurer:** Steve Edwards
- **IT Officer:** Pat Caron

Ron Grant reported 15 verified votes, including proxies. This represented roughly 43% of the membership and exceeded the required quorum.

Pat Caron noted that he is located in **Espanola, Ontario, Canada**, making the DPRG board international.

## RoboRama 2026 Competition Planning

The group confirmed that the May indoor RoboRama competition will continue. Proposed contests include:

- Six Can
- Quick Trip
- Four Squares
- Barrel Racing
- Mini Sumo
- Advanced Line Following
- Search and Retrieval, if competitors are interested

There and Back was also discussed as a useful entry-level event for new robot builders.

### Line-Following Events

- Mark Reynolds intends to defend his previous line-following win by entering the advanced event.
- Mike Williamson is considering adapting a second mini-sumo robot for line following.
- The advanced course introduces more difficult track features than the basic event.
- The Challenge course remains available, although it has reportedly been completed only in simulation and not yet successfully on the physical course.

### Proposed Rule Changes

Doug Paradis outlined several possible changes:

- Every robot must meet a defined minimum performance threshold before qualifying for a prize.
  - A line follower might need to follow the line through at least the first curve.
  - A Six Can robot might need to place at least one can successfully.
- Consider limiting each competitor to two robots per event.
- Alternatively, allow unlimited robots but limit each competitor to one prize per event.
- Require at least two entrants for an event to count as a competition.
  - A sole entrant could still run as a demonstration and receive an award equivalent to third place.
- Continue exploring new events, including an obstacle-avoidance course with an array of upright barriers.

These proposals remain open for discussion during future Robot Builders Night Virtual meetings.

### Trophies

- The group favored returning to the transparent fluorescent acrylic trophy style.
- Access to suitable laser-cutting equipment should make production easier.
- Trophy colors have not historically corresponded consistently to placement, and no final standard was adopted.

## Remote Competition

Remote participation will continue to be supported for RoboRama.

- Pat Caron plans to organize participation from a recreation center in Espanola and advertise the event locally.
- Doug suggested contacting schools or science teachers to encourage student participation.
- Participants discussed allowing remote robots to compete directly against Dallas entrants when equivalent courses can be established.
- Pat favored direct competition rather than receiving an uncontested remote award.
- Line following was identified as especially suitable for distributed competition because identical course artwork can be printed in multiple locations.
- Shipping a printed course from the United States may be more affordable than having a complete course printed in Canada.

## UTD Comet Robotics Event

The group discussed attending a UTD Comet Robotics event scheduled for **Saturday, March 14, 2026**.

- The event is expected to include one-pound plastic, one-pound, and three-pound combat robots.
- Mini-sumo activity may also be available.
- Mike Williamson expressed interest in bringing his mini-sumo robots for testing.
- The group noted that SPARC-related rules may include or encourage partially autonomous combat robotics.

## Proposed Technical Presentations for 2026

Participants developed a preliminary list of presentation topics.

### Mod Linker

Mark Dombrowski volunteered to present **Mod Linker**, short for “module linker,” once the project is further developed.

- The project is intended to simplify communication among robot modules.
- It may also help builders design and share modular electronics more effectively.

### Robot Communication Interfaces

A proposed introductory tutorial would compare common peripheral interfaces:

- I²C
- SPI
- UART
- CAN bus

The talk would help builders progress beyond direct GPIO connections and understand how to connect more sophisticated sensors, motor controllers, and distributed modules.

### ROS 2 Basics and Workspace Management

Suggested ROS topics included:

- Establishing simple ROS 2 communication between a PC, Raspberry Pi, or microcontroller.
- Keeping the demonstration focused and approachable.
- Structuring a ROS workspace correctly.
- Using GitHub without committing generated files or an entire ROS installation.
- Selecting appropriate source, map, configuration, and ancillary directories.
- Using `.gitignore`.
- Comparing Docker-based and native ROS installations.

Mike Williamson may present his non-Docker workflow, while Paul Bouchier may be able to contribute Docker and GitHub guidance.

### Artificial Intelligence

At least two AI presentations were proposed:

1. **Moving beyond “vibe coding”**
   - Effective use of coding agents.
   - Progressing from informal prompting toward more disciplined software development.

2. **Local versus cloud AI for robots**
   - Object detection and computer vision.
   - Running models locally on a Raspberry Pi or robot computer.
   - OpenCV and related tools.
   - Possible application to a future search or object-detection competition.

The group mentioned Kareem, Steve, and Paul as possible contributors.

### Structural Design for 3D Printing

Mark Dombrowski offered to prepare a CAD-platform-independent talk about designing functional robot parts for 3D printing.

Potential subjects include:

- Strength and print orientation.
- Structural components and mechanisms.
- Fits, clearances, and tolerances.
- Modular designs that avoid support material.
- Threaded inserts.
- Material selection and the limitations of PLA.
- Designing linear rails and other mechanical assemblies.

Although Mark uses Fusion 360, the methods would also apply to Onshape and other CAD systems.

### Robot Design Reviews and Club Robot

Additional presentation ideas included:

- A detailed review of Scott’s indoor competition robot.
- Mechanical precision, electronics, and software practices that contribute to reliable performance.
- Lessons learned from developing a standard club robot.
- Revisiting useful topics such as KiCad, CAD, and 3D modeling.
- Creating robot simulations, possibly using Processing.

The final schedule will remain flexible so DPRG can respond to new technologies, speakers, and tour opportunities.

## Project-Focused Robot Builders Night Out

Mark Reynolds proposed restarting regular in-person Robot Builders Night Out sessions, possibly weekly or every other week.

The group agreed that these meetings would be most effective if they focused on a shared project rather than having everyone bring unrelated work. Advantages include:

- Tools and materials can remain ready at the meeting location.
- Participants spend less time packing and unpacking.
- Members can collaborate on clearly assigned tasks.
- Remote members can contribute software or modules with defined interfaces.

## Restoring the Club Robot Robie

Robie was proposed as the primary shared project for the renewed builder nights.

Possible work includes:

- Completing or redesigning the second arm.
- Improving safety and blocked-joint detection.
- Adding better vision.
- Adding speech or voice recognition.
- Improving overall functionality for public demonstrations.
- Defining modules that remote participants can develop and test.

The group favored completing the existing full-size Robie before building a smaller successor. Robie’s large size makes the robot an effective attraction at outreach events such as Moon Day.

A separate mobile robot could eventually travel through an event venue, invite people to visit the DPRG display, and use supervised navigation to avoid visitors.

## Website, Tutorials, and Documentation

Mark Reynolds would like DPRG to publish more project and tutorial content.

- The latest tutorial currently visible on the website dates from approximately 2022.
- Members were encouraged to turn useful discoveries from meetings and projects into written documentation.
- AI-assisted documentation was suggested as a way to reduce the burden on hobbyists.
- The website is reportedly slow, and the club may need to ask its hosting provider for additional resources or consider paid hosting.
- Older Robot Builders Night Virtual recordings contain valuable information but often lack transcripts or AI summaries.
- The group discussed whether older videos could be transcribed and summarized retrospectively to make their technical content easier to locate.

## Administrative Notes

- The regular Tuesday Robot Builders Night Virtual meetings will continue.
- A board meeting originally planned after this call was postponed until additional officers, including Steve Edwards and Paul Bouchier, are available.

# Conclusions and Insights

- DPRG entered 2026 with a unanimously elected leadership team and stable participation across virtual and in-person activities.
- RoboRama will continue in May with familiar events, advanced line following, mini sumo, and potentially a search-and-retrieval contest.
- Competition rules will likely be refined to require meaningful minimum performance and to prevent uncontested or duplicate prize awards.
- Remote competition remains a priority, with interest in integrating remote entrants directly into the Dallas standings.
- The proposed 2026 technical program emphasizes practical robot-building skills: communication buses, ROS 2, AI, structural 3D printing, simulation, and modular electronics.
- In-person builder nights should be revived around a shared project, with restoration and enhancement of Robie as the leading candidate.
- Website performance, project documentation, and preservation of knowledge from older meeting videos are important infrastructure goals for the year.

## Referenced Links

### Mark R

- [StickersBanners.com](https://stickersbanners.com/)  
  Discussed as a possible vendor for printing vinyl line-following courses. Shipping cost and availability for Canadian participants need to be confirmed.

- [DPRG Line Following Contest Repository](https://github.com/dprg/Contests/tree/master/Line%20Following)  
  Contains line-following course files and related contest resources suitable for producing matching courses at local and remote competition sites.
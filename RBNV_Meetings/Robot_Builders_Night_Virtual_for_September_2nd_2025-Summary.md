# Robot Builders Night Virtual for September 2nd, 2025

## Introduction
The virtual meetup focused primarily on updates and discussions of robotics projects, particularly those related to obstacle avoidance and sensor technologies in autonomous robots.

## Main Discussion Points

### Mike Williamson's Robot Update
- **Obstacle Avoidance:** Mike has been improving his robot's ability to traverse indoor environments using multi-point time-of-flight (TOF) sensors arranged in an 8x8 array. These help the robot avoid obstacles like walls and better approach targets like cones.
- **Sensor Calibration Issues:** Participants discussed issues related to erroneous sensor readings, often due to reflections and calibration, particularly when sensors pick up speckles not corresponding to actual obstacles.
- **Environmental Navigation:** Mike’s robot uses a combination of LiDAR for navigation and TOF sensors for detailed obstacle detection. Challenges remain in filtering sensor data to eliminate false positives, such as irrelevant speckles above the floor.
- **Contribution to Configuration:** Doug P. and others suggested tactics like angling ultrasonic sensors slightly to improve accuracy and reduce erroneous reflections.

### RoboColumbus Competition Preparations
- **RTK and GPS Strategies:** The group explored the use of RTK GPS systems for competitions, weighing the benefits and challenges of accuracy versus system complexity. Differentiation of RTK GPS from traditional GPS and their implementation in robot navigation were key points.
- **Competition Rules Clarification:** Doug and others clarified aspects related to GPS and waypoints. Discussions revolved around allowable technologies, use of RTK GPS, and strategic planning regarding waypoint management during competitions.
- **Scoring System:** The RoboColumbus scoring was discussed, highlighting how challenges like using zero waypoints or no GPS can add complexity—and potentially additional points—to the contest.

### Technology and Tools
- **DF Robot RTK GPS Kit:** Doug P. showcased a new RTK GPS kit from DF Robot, noted for its affordability and simplicity, which could be advantageous for newcomers and educators.
  
### Innovative Concepts
- **Automated Trash Bins:** A humorous project involving robots as moving trash bins with smart detection systems sparked discussions on practical applications and the over-engineering of simple tasks.

## Conclusions and Insights
- The continuous development of more sophisticated sensor arrays is crucial for improving obstacle navigation. Collaborative advice and troubleshooting are integral to solving persistent issues like sensor noise and false positives.
- Strategic use of GPS and RTK systems can greatly impact the outcomes in competitive robotics, with ongoing discourse beneficial for refining both robot capabilities and competition rules.
- There's a community interest in potentially merging robotics with creative problem-solving to showcase skills, even in whimsical applications like moving trash cans. However, the practicality and cost of such projects remain topics of reflection.

## Referenced Links by Contributor
- **Mike Williamson:**
  - Shared insights into TOF sensors, specifically tagging models VL53L8CX and VL53L5CX for their applications and differences in light tolerance.
  
- **Doug P.:**
  - Introduced the DF Robot RTK GPS Kit, highlighting its potential for direct application in competition settings where exact positioning is key.

The meeting conveyed both technical advancements and a community spirit in overcoming challenges together, showcasing the iterative nature of robot development.
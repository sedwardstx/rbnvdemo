# Robot Builders Night Virtual for October 21st, 2025

## Introduction
The Robot Builders Night Virtual for October 21, 2025, commenced with Paul Bouchier welcoming participants and outlining the agenda which included DPRG news, discussions on IMU problems, and navigation strategies for robots with obstacle avoidance and localization.

## Main Discussion Points

### DPRG News
- The upcoming monthly meeting on October 25th will feature two presentations: 
  1. A continuation of a Git and GitHub talk.
  2. A presentation by Thomas Meshmid from HBRC on an AI-generated video interview demonstrating AI's potential and challenges.
- Paul Bouchier sought volunteers to manage YouTube recordings in his absence starting in November.

### Robot IMU and Localization Challenges
- Mike Williamson discussed challenges with integrating sensors for robot localization using EFK modules:
  - Faced issues with IMU calibration, specifically with yaw using the BN085 sensor.
  - Experimented with different rotation vectors but struggled with delay discrepancies between IMU and wheel odometry.

### Navigation and Obstacle Avoidance
- Discussions on utilizing lidar and time of flight sensors for outdoor navigation and obstacle detection:
  - Ray Casler and others shared experiences with various lidar models and sensors for effective outdoor robot navigation.
  - Exploration of ways to optimize sensor calibration and minimize impact from environmental factors like sunlight.

### RTK GPS and Waypoint Navigation
- Ray Casler shared experiences with setting up RTK GPS but noted challenges in maintaining calibration and executing correct waypoint navigation.
- Discussions on whether to incorporate predefined waypoints or rely on GPS and sensor data for dynamic navigation.
- Jason C inquired about strategies for implementing waypoints alongside GPS to correct drift using an EKF filter in Ross environments.

## Conclusions and Insights
- Robots can achieve more reliable navigation by refining sensor calibration techniques and considering environmental influences.
- Balancing between using predefined waypoints and adaptive sensor data appears crucial for effective obstacle avoidance and course navigation.
- Adapting to unexpected technical challenges such as Wi-Fi bandwidth issues during live presentations remains a constant consideration for virtual meetings.

## Referenced Links
- **Ed Mart shared**: [Adafruit Product Link](https://www.adafruit.com/product/4441) for lidar components.
- **Ted Meyers shared**: [SparkFun Lidar Link](https://www.sparkfun.com/lidar-lite-v3hp.html)
- **Paul Bouchier shared**: GitHub repositories for robot navigation script:
  - [Scripted Bot Driver](https://github.com/PaulBouchier/scripted_bot_driver)
  - [Scripted Bot DRI](https://github.com/PaulBouchier/scripted_bot_dri)

Participants engaged actively in discussing ways to tackle current issues in robotics, emphasizing collaborative problem solving and knowledge sharing as essential for innovation in DPRG meetings.


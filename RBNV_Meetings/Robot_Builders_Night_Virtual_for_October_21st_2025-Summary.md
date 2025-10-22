# Robot Builders Night Virtual for October 21st, 2025

## Video @ https://youtu.be/w79pildtY4M

## 

## Main Discussion Points

### DPRG News

* The upcoming monthly meeting on October 25th will feature two presentations:

  1. A continuation of a Git and GitHub talk.
  2. A presentation by Thomas Messerschmidt from HBRC on an AI-generated video interview demonstrating AI's potential and challenges.

### Robot IMU and Localization Challenges

* Mike Williamson discussed challenges with integrating sensors for robot localization using EKF modules:

  * Faced issues with IMU calibration, specifically with yaw using the BN085 sensor.
  * Experimented with different rotation vectors but struggled with delay discrepancies between IMU and wheel odometry.

### Navigation and Obstacle Avoidance

* Discussions on utilizing lidar and time of flight sensors for outdoor navigation and obstacle detection:

  * Ray Casler and others shared experiences with various lidar models and sensors for effective outdoor robot navigation.
  * Exploration of ways to optimize sensor calibration and minimize impact from environmental factors like sunlight.

### RTK GPS and Waypoint Navigation

* Ray Casler shared experiences with setting up RTK GPS but noted challenges in maintaining calibration and executing correct waypoint navigation.
* Discussions on whether to incorporate predefined waypoints or rely on GPS and sensor data for dynamic navigation.
* Jason C inquired about strategies for implementing waypoints alongside GPS to correct drift using an EKF filter in Ross environments.

## Referenced Links

* **Ed Mart shared**: [Adafruit Product Link](https://www.adafruit.com/product/4441) for lidar components.
* **Ted Meyers shared**: [SparkFun Lidar Link](https://www.sparkfun.com/lidar-lite-v3hp.html)
* **Paul Bouchier shared**: GitHub repositories for robot navigation script:

  * [Scripted Bot Driver](https://github.com/PaulBouchier/scripted_bot_driver)
  * [Scripted Bot DRI](https://github.com/PaulBouchier/scripted_bot_dri)




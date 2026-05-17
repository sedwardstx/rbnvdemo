# Robot Builders Night Virtual for May 12th, 2026

## [DPRG RBNV - Robot Builders Night Virtual - May 12, 2026 - YouTube](https://www.youtube.com/watch?v=YHTYHmDaNxw)

## Key Discussion Topics

### **Club Announcements and Event Logistics**

- **Roborama 2026:** The annual Roborama competition will take place on May 23, featuring events like Line Following, Barrel Racing, and Sumo. A Texas Robot Combat "Robot Rodeo" is also scheduled for May 30.  Doug Paradis volunteered to cut translucent acrylic trophies, Paul Bouchier agreed to design and print certificates, and Mark R and Paul coordinated ordering pizza for the event.
  
  
- **Moon Day:** Mark R noted that the club needs a volunteer to lead the July 18 Moon Day event at the Fontes of Flight Museum due to scheduling conflicts, though he will still send his robot float display.
  
  
  
  ## Presenters

**Paul B:** demonstrated his Moberry robot running on an ESP32 microcontroller. Because his robot software expected quadrature encoders but his hardware used single-channel encoders, he successfully configured the ESP32's pulse counter to use channel B as a direction control. This allowed him to successfully publish odometry data for the Robot Operating System (ROS).  Black star ★



**Mike W:** discussed solutions for detecting cans on shiny floors, which cause reflections that trick the camera's aspect ratio calculations. Solutions ranged from using paper inserts in the cans to block reflections, setting a specific height "region of interest" for the camera, to Doug Paradis's suggestion of using simple blob detection paired with a distance sensor, taking advantage of the competition's predictable white-wall environment.



**Pat C:** shared progress on bypassing standard development environments to run Python on a microcontroller. He uses `uv` to manage virtual environments and a Redis server for background communications between multiple scripts.



**Chris N:** demonstrated his progress updating a Lidar "dewarping" (motion compensation) script from ROS 1 to ROS 2. He showed that when a robot rotates, the Lidar scan warps heavily and the odometry drifts. Mike Williamson added that accelerating a robot's rotation changes the momentum of the spinning Lidar device. This inertial disturbance takes the Lidar's internal compensation loop up to 10 seconds to stabilize, causing severe mapping inaccuracies.

**Carl O:** suggested a mechanical fix to this software problem: placing a physical barrier (about 1.5 pixels wide) on the robot to block the Lidar beam at a "location zero". This intentional dropout creates a predictable index point, allowing the software to reliably calibrate the data upon each rotation.



**Navigation Algorithms and AI Hardware**

**Karim V:** presented an analysis of the Pure Pursuit (RPP) navigation algorithm. He concluded that while it works well in open fields, it relies on projecting "carrots" (waypoints) forward and lacks specific cross-track correction. As a result, the geometry-based algorithm oscillates and struggles to maintain a centerline on narrow paths, frequently driving the robot into side brush.



**Doug P:** unboxed a new compact Open Machine Vision AE3 AI camera he backed on Kickstarter. He also shared that he has been utilizing the AI tool Claude to program his "Little Andy 2" robot, noting that the AI is exceptionally good at pinpointing and fixing compiler errors. 



**Paul B:** introduced the $34 Unhiker K10 AI camera, which features a microphone and speakers; he is exploring its use for facial recognition so his robot can automatically rotate to center a human face and give a verbal greeting.Cost considerations were noted, particularly in regard to the TOF sensor modules.



## Referenced Links

- **Pat Caron provided**:
  
  - [OpenMV AE3 Camera](https://openmv.io/collections/cameras/products/openmv-ae3)

- **Paul Bouchier provided**:
  
  - [STMicroelectronics TOF Modules](https://www.mouser.com/new/stmicroelectronics/stmicroelectronics-vl53lp-tof-modules/?srsltid=AfmBOorTtypKC5GdnpewCccEdz2qZeSI7XKHAUizh9B_tt6hW42J8le8)

- **Mark R provided**:
  
  - [Unihiker K10 Wiki](https://www.unihiker.com/wiki/K10/)
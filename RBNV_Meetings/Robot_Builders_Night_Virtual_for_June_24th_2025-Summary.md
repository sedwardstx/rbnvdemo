# Robot Builders Night Virtual for June 24th, 2025

## Introduction
The latest Robot Builders Night Virtual meeting covered a range of topics from upcoming events at the DPRG to technical discussions about robotics software and hardware challenges. Enthusiasts from various backgrounds shared their insights and ongoing projects, leading to an engaging and informative session.

## Main Discussion Points

### DPRG News and Upcoming Events
- Paul Bouchier announced a visit to a Robot Lab scheduled for Saturday. The discussion included confirmations of attendance and potential expansions to accommodate more participants.
- Conversations touched on the types of robots featured at the lab, leaning towards warehouse and retail-focused robotics rather than agricultural models.

### Technical Presentation on Zeno
- Paul Bouchier presented on the integration and benefits of Zeno and Zeno Pico as alternatives to DDS in ROS for improved network communication in robotics, especially in unreliable multicast environments.
- Zeno replaces the DDS layer for message passing between ROS systems, offering a lower overhead and better reliability, particularly in Wi-Fi networks where DDS struggles.

### Challenges and Solutions with ROS and Network Configurations
- Participants including Mike Williamson and Paul Bouchier shared insights on difficulties faced with ROS installations and network configurations, such as issues with multicasting over Wi-Fi.
- Solutions included using specific network configurations and software like X11 VNC for accessing graphical interfaces remotely.

### New Robotics Hardware and Software Innovations
- Tom Crawford introduced new acquisitions, including an STM32 ARM microcontroller and vintage VEX Robotics hardware, discussing their potential in educational and hobbyist robotics.
- Discussion about Robot C, a software platform developed by Dick Swan for programming robots using C language, highlighting its utility and history.

### Experiments with PoE Cameras and Microcontrollers
- Tom Crawford showcased a new power-over-Ethernet (PoE) camera, illustrating its value for home security and potential robotic applications, given its high resolution and AI capabilities for human detection.
- Experiments with Arduino IDE and STM32 hardware indicate a trend towards integrating more sophisticated, low-cost components in personal projects.

### Construction and Testing of Autonomous Vehicle Controllers
- Mike Williamson shared steps towards building a controller for a robotic vehicle, detailing challenges in capturing telemetry data from an ESC motor controller.
- Discussion covered protocols for data exchange and considerations for reliable, real-time feedback mechanisms in robotics applications.

### VEX Robotics and Educational Use
- Tom Crawford and Karim Virani discussed the historical context and applications of VEX Robotics systems in education and competition, including connections to the FIRST Robotics Competition.
- Emphasis was placed on how these platforms provide solid educational experiences in building and programming robots.

## Conclusions and Insights
- The integration of new technologies and troubleshooting within robotics requires collaborative effort and sharing of best practices among enthusiasts.
- Interest in emerging tools like Zeno reflects a common desire to move past limitations of existing technologies like DDS in favor of more efficient alternatives.
- Educational robotics continues to play an essential role in developing problem-solving skills and a deeper understanding of engineering principles.

## Referenced Links
- Paul Bouchier:
  - Presentation on [Zeno and Zeno Pico](https://zenoh.io) - for improved DDS replacement in ROS
- Tom Crawford:
  - Overview of using power over Ethernet (PoE) for high-resolution cameras in robotics.
- Karim Virani:
  - Discussion of VEX and FIRST Robotics history and their roles in education.

The meeting highlighted advancements and ongoing challenges within the robotics community, showcasing the collaborative spirit essential for innovation and progress.
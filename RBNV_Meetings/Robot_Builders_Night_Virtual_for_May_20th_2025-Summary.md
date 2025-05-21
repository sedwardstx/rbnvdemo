# Robot Builders Night Virtual for May 20th, 2025

## Introduction
The May 20th, 2025 edition of Robot Builders Night Virtual centered around upcoming robotics events, project updates, and technical discussions. Key topics included preparations for the Roboama event, insights into ROS 2 migration, and technical challenges and solutions in using MicroPython on various hardware.

## Main Discussion Points

### Roboama Preparation
- **Event Details**: Roboama is scheduled for Saturday, with video recording for remote participants.
- **Setup and Participation**: Attendees discussed the event setup, including a planned visit to Robot Lab in June and participation in Moon Day in July.

### Technical Challenges and Solutions
- **MicroPython Performance Issues**: Dave Ackley discussed challenges with MicroPython’s performance, particularly when running on the ESP32, which is significantly slower than native C/C++.
- **Python on ESP32 and Pico**: Tom Crawford highlighted performance differences using MicroPython on the ESP32 versus the Pico, noting the ESP32 has challenges with digital interrupts due to MicroPython’s implementation.
- **Alternative Solutions**: Integrating Arduino for performance-critical tasks was recommended, utilizing serial interfaces which perform effectively on MicroPython.

### ROS 2 Migration
- **Chris N’s Project**: Transitioning a robotics platform from ROS 1 to ROS 2, Chris N. shared hurdles in refactoring code, noting improvements with new installation on Ubuntu.
- **Key Considerations**: Discussion touched on maintaining old coding styles within the new ROS 2 framework and exploring class structures versus node handles.

### Barrel Racing Event
- **Regulations Update**: Doug Paradis and Ponder SomeMore discussed amending rules for barrel racing, including the option for extending the start line and addressing competition constraints.
- **Community Engagement**: Encouragement for community involvement in events with suggestions for prize incentives.

### Open Mic & Technical Queries
- **Hardware Troubleshooting**: Chris N. sought advice on a LIDAR setup, revealing mismatches in wiring and power configuration, sparking discussions on signal lines and hardware grounding.
- **MicroPython Functionalities**: Strategies for optimizing sensor data processing on the Raspberry Pi Pico.

## Conclusions and Insights
- **Collaboration and Sharing**: The meeting showcased the value of collaborative troubleshooting and shared experiences in overcoming technical challenges.
- **Event Engagement**: Emphasized the importance of preparation for successful participation in competitive robotics events like Roboama.
- **Continuous Learning**: Highlighted ongoing education in shifting technology paradigms such as ROS 2 migration and efficient use of MicroPython.

## Referenced Links
- **Ponder SomeMore**: 
  - [Barrel Racing Discussion on Discord](https://discord.com/channels/1211398208865968170/1352418320401301647/1374448055943958689)

This summary covers the essence of the May 20th, 2025, meeting, encapsulating the collaborative spirit and enthusiasm for robotics challenges and learning.
# Robot Builders Night Virtual for May 5th, 2026

## [DPRG RBNV - Robot Builders Night Virtual - May 5, 2026 - YouTube](https://www.youtube.com/watch?v=4aPnJnQjTw4)

## Club News

**DPRG** is hosting **RoboRama 2026** set take place at the DMS on Saturday May 23rd. Events include:

    - Quick Trip
    - Line Following - Advanced
    - Barrel Racing
    - 6-Can
    - 4 Square
    - Sumo  

**Texas Robot Combat - Robot Rodeo 2026**

Will take place Saturday, May 30th.  Fighting Open Ants, Plastic Ants, and Open Beetles. Free to all ages of the public.
Fights start at 10:30 am. Be there early for best seating.
Hosted by REV Robotics 2941 Commodore Dr, Ste 110 Carrolton, TX 75052

## Presenters

### **Lidar Motion Compensation**

**Mike W** presented a custom algorithm correcting lidar scanning errors caused by linear and angular robot motion. It compensates for these errors based on velocity and scan time, which improved his robot's barrel racing speed from 0.15 m/s to 0.5 m/s. Others suggested these errors might stem from system latency and IMU update rates, and proposed building a motorized calibration rig to gather ground-truth rotation data.



**AI and LLM Coding Integration**

- The team discussed AI coding tools, noting that LLMs are most effective when allowed to compile and test their own output. However, strict guardrails are necessary to prevent the AI from accidentally commanding physical robots to move during testing. To improve output, users should write a rough draft and iteratively refine the prompt with the AI. Running the open-weight Gemma 4 model locally was highly recommended as a free alternative to paid subscriptions.
  
  

**Moberry Robot Lawn Mower Prototyping**

- **Paul B** demoed the responsive Moberry control board, which uses a Raspberry Pi 4 and a Micro-ROS agent communicating with an ESP32 to drive motors. To run ROS smoothly on a 4GB Pi 4, utilizing swap space and an SSD is highly recommended. Seeking alternatives to expensive GPS units, the team discussed Chinese L1/L5 RTK GPS modules that cost around $60 to $80, though they might require writing custom ROS drivers.  Black star ★
  
  

**Hardware Prototyping and 3D Printing**

- Tom Crawford showcased custom gear motors for a large outdoor robot, featuring T5 pulleys and IR sensors for potential quadrature encoding. He also successfully restored the print quality of his 10-year-old 3D printer by manually re-leveling the bed, reducing the variance down to 0.15mm.
  
  

**Ed M** - Robotic links

- https://www.facebook.com/share/v/1DyBVYmmM8/
- https://www.facebook.com/share/v/14XPPqsQQBi/

## Referenced Links

- **Chris N ** 
  
  - [De-warping Lidar Motion Compensation](https://github.com/nettercm/lidar_dewarping)

- **Ponder SomeMore**
  
  - [Waveshare LC29H GPS HAT](https://www.waveshare.com/lc29h-gps-hat.htm?sku=25280)

- **Philip Foster**
  
  - [Waveshare Dual-Band GPS on Amazon](https://www.amazon.com/Waveshare-Dual-Band-Positioning-Technology-Augmentation/dp/B0CGX7MRRC)
    
    

Black star ★ (Significant progress)
Gold star ⭐ (Autonomous running)
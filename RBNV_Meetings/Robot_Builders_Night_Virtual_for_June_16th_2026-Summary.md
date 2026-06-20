# Robot Builders Night Virtual for June 16th, 2026

## [RBNV 2026 June 16/2026 - YouTube](https://www.youtube.com/watch?v=HAHrxbgE138)

## Presenters

**Ray C** - demonstrated a platform utilizing hoverboard hub motors driven by three-phase brushless motor boards. Because the motor drivers lack built-in speed regulation, Ray shared his custom 3D-printed shells that mount Hall effect sensors to act as magnetic encoders, which will help close the control loop for better velocity control. He also noted that the tires on these hub motors can be replaced or modified for better grip.
     
**Paul B** - presented a detailed field comparison between a \$73 Waveshare LC29H RTK GPS receiver and a \$300 U-blox ZED-F9P. By testing both units simultaneously around his yard, Paul demonstrated how accuracy degrades during external RTK correction dropouts and under environmental obstructions like dense crepe myrtle trees. The group discussed that while budget GPS hardware is highly capable, a robust navigation system requires multi-sensor localization.
Paul also shared a link to an ETH Zurich online lecture series on advanced robotics, which covers topics like imitation learning, reinforcement learning, and generative models.
  
**Karim V** - showcased a \$400 Unitree LiDAR sensor that provides a full point cloud for obstacle detection. He discussed his ongoing efforts and challenges in using Cloud Compare software to filter the data and accurately align the sensor's point of origin.



## Conclusions and Insights

- RTK GPS systems offer precise location tracking, making them valuable for robotics applications requiring high accuracy.
- Determining the necessity of a base station is important for cost-effective implementation.
- Continuing education, such as the Robot Learning course, can enhance participants' knowledge and skills in robotics.

## Referenced Links

- Paul Bouchier provided the following links:
  - [lc29h_da RTK GPS Driver GitHub](https://github.com/PaulBouchier/lc29h_da_rtk_gps_driver) - Repository for RTK GPS driver.
  - [ETH Zurich Robot Learning Course](https://cvg.ethz.ch/lectures/Robot-Learning/) - Educational resource for robotics learning.
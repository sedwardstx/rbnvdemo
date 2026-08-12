# Robot Builders Night Virtual for August 11th, 2026

## [RBNV 2026 Aug 11/2026 - YouTube](https://www.youtube.com/watch?v=-EHmGGm8uLY&pp=0gcJCckLAYcqIYzv)

## Key Discussion Topics

- **Autonomous Navigation and Sensor Tuning:** The team successfully demonstrated an outdoor robot navigating to a target cone. Key adjustments included fabricating a 5-degree downward mounting wedge for the LiDAR to overcome height and suspension limits, resolving a loose Inertial Measurement Unit (IMU), and fusing long-range camera tracking with stable short-range LiDAR and time-of-flight sensors.
- **Firmware Integration & Custom Driver Development:** Members discussed integrating an IMU with an ESP32 microcontroller using Micro-ROS, implementing a 6-axis mode to handle orientation, and utilizing a soft-reset workaround for stable readings. Additionally, a custom driver developed for the LC29H RTK GPS receiver was presented. The group noted the diagnostic limitations of this GPS module (lacking a clear RTK fix indicator) compared to U-blox modules, which remain the preferred option for rapid progress.
- **Telemetry and Machine Learning Data:** A demonstration showed GPS telemetry and satellite counts visualized across multiple terminal windows using ZeroMQ. The group also discussed training cone detection models to recognize partial views and shared a valuable public resource featuring 40,000 hours of robot data for machine learning.
- **Bench Tools and Hardware Hacks:** The club has acquired a new dual-channel 30V/5A bench power supply and a multi-channel oscilloscope. Members shared tips on converting old computer power supplies into bench units, noting that a 5V rail load (like a 12V incandescent bulb) is required.
- **Security and Micro-Displays:** The meeting wrapped up with discussions on configuring secure, standalone outdoor cameras with static IPs (blocked from external internet access) and exploring cheap ESP32 touchscreen display modules (such as the $10 "cheap yellow display") for robot status monitoring.

## Referenced Links

- **Pat Caron:** 
  - [datasets.bot](https://datasets.bot/) - A repository for datasets critical for robotics training and development.
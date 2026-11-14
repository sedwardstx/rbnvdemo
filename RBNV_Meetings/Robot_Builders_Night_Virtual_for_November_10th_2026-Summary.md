# Robot Builders Night Virtual for November 10th, 2026

[RBNV Video Nov 10/2026](https://www.youtube.com/watch?v=Fg2cMWi7yuM)

## DPRG Club Business

- RoboColumbus 2026 - There is less than 2 weeks until the event. Are you ready? The annual competition date is set for Saturday, November 21st, moving one week earlier to avoid interference with Thanksgiving travel plans. Spectators are welcome to attend even if they do not have a robot entered in the contest. Reach out to Paul B or Mark R for event location details.

## DPRG Club News -

### Presenters

- **Mike W** - Mike tested GPS and odometry data fusion using a Raspberry Pi 5 with an SSD.

- Raw GPS tracking demonstrated better accuracy than filtered odometry data during outdoor runs.

- LiDAR and camera sensors enabled the robot to detect cones and navigate around obstacles.

- Mike expanded waypoint planning scope to 220 meters to resolve previous path calculation limits.

- Continuous battery runtime testing demonstrated stable operation for up to 2 hours.

- **Doug P** - Doug unveiled the 2026 competition mug featuring a robot viewpoint graphic.

- Competitors earn a mug by scoring at least 1 point in the event.

- **Tom C** - upgraded analog sampling to 1,000 samples per second to mitigate 120 Hz power supply ripple noise.

- Tom implemented interrupt-driven non-blocking analog-to-digital conversion to reduce CPU usage on the Arduino Nano.

- Thermal load calculations indicated heat sink dissipation limits of 11 to 12 watts.

- Operating tests measured approximately 5 watts of thermal power transferring into the heat sink.

- Tom Crawford formulated equations to estimate transistor junction temperature using collector current and base-emitter voltage.

- Measurements recorded case temperatures reaching 75 degrees C and junction temperatures hitting 81 degrees C.

- Collector current climbed from 310 milliamps to 550 milliamps as the transistor heated up.

- **Ray C** - updated us on how he mounted a TF mini sensor on a servo to scan for obstacles.

- An ESP32C3 microcontroller processes sensor data to detect obstacles up to 2 meters away.

- Ray Casler installed a local voltage regulator to resolve power sags from the servo.

- Gold Builder replaced a bent motor shaft at no cost to the project.

- **David S** - introduced an AI assistant to present recent robotics industry news highlights.

- Tesla targeted high-volume production for its Optimus factory in Austin by summer 2027.

- Foxconn deployed humanoid robots on its Nvidia AI server manufacturing line in Houston.

- The AI news presentation consumed an estimated tens of watt-hours of energy.
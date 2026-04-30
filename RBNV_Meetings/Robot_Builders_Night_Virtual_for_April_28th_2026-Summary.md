# Robot Builders Night Virtual for April 28th, 2026

## [DPRG RBNV - Robot Builders Night Virtual - April 28, 2026 - YouTube](https://www.youtube.com/watch?v=2coWEPqAPEc)

### DPRG News

**Club Competitions* - DPRG is hosting RoboRama 2026 set take place at the DMS on Saturday May 23rd. Events include:
    - Quick Trip
    - Line Following - Advanced
    - Barrel Racing
    - 6-Can
    - 4 Square
    - Sumo  
          


**ICYMI - DPRG April Monthly Mtg** The Sensori Robotics team showcased their UniTree Go2 Robot + some great robot demos!

**Texas Robot Combat Robot Rodeo 2026** - Will take place Saturday, May 30th.  Fighting Open Ants, Plastic Ants, and Open Beetles. Free to all ages of the public.
Fights start at 10:30 am. Be there early for best seating.
Hosted by REV Robotics 2941 Commodore Dr, Ste 110 Carrolton, TX 75052
 

## Presenters

 **Paul B** - Robotic Mower Mechanics and Micro ROS Integration** Paul showcased a robotic mower blade assembly utilizing a brushless DC motor with an estimated 20-inch total cut width. He advised starting the counter-rotating blades at 2,800 RPM in random directions while the mower is already moving to maximize blade wear and prevent motor stalls in tall grass. Paul also successfully demonstrated driving the mower via ROS joystick commands using an ESP32 running micro ROS. To overcome the limitation of a single-channel encoder, he detailed a workaround using the ESP32's PCNT module to increment or decrement counts based on the intended motor direction.  Black star ★

**Mike W** - Mike investigated a short circuit that destroyed the RP2040 processor on his rotating framed art project. He deduced that the frame's heavy, highly-geared motor was likely shifted manually, generating a back EMF that over-volted the 5-volt line. To prevent future surges, he plans to add a Schottky diode. Members recommended techniques from the "Mr. Solder Fix" YouTube channel for easily unsoldering the damaged chip. Mike also shared a simple $5 power supply meter he attached to his robot for instant visual battery voltage readouts.

**Harold P** - shared his ongoing struggles to stabilize a balancing bot by manually tuning its PID loops and Kalman filters. To help calculate the complex covariance matrices, he experimented with chaining AI prompts between Copilot in Windsurf and Visual Studio Code. Harold also expressed frustration with PlatformIO mismanaging COM ports and project targets when handling multiple projects in a single workspace. Members suggested workarounds, such as using Linux symbolic links (symlinks) to reliably target specific ports, or utilizing environment variables (`ENV`) and command line flags to strictly control the build targets.



## Referenced Links

- **Mike Williamson:**
  - [YouTube Video](https://www.youtube.com/watch?v=OJg_E0_gI6k) - Resource related to the discussion, potentially providing a visual explanation or demonstration.
  - [Amazon Link](https://www.amazon.com/dp/B0FD9KQN1Q?ref=ppx_yo2ov_dt_b_fed_asin_title) - Presumably links to a product or tool relevant to the discussion, providing practical examples or options for robotic solutions.

This meeting facilitated a detailed exploration of technical aspects of robotics, emphasizing both theoretical understanding and practical application methods.



### Stars

Black star ★ (Significant progress)
Gold star ⭐ (Autonomous running)
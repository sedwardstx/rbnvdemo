# Robot Builders Night Virtual for October 28th, 2025

## Video @ [DPRG RBNV - Robot Builders Night Virtual - October 28, 2025 - YouTube](https://www.youtube.com/watch?v=Dxs7oF5VJ44)

## Main Discussion Points

### Tom Crawford's Doorbell System Project

- **Objective**: Upgrading an old doorbell system to play real music.
- **Technical Details**: Utilization of an ESP 8266 microcontroller with an 8-bit DAC and a shift register configuration. Wave files are converted using Audacity to 8-bit mono format for playback via a LittleFS file system.
- **Challenges Encountered**: Issues included variable latency of LittleFS and integration of Arduino with ESP 8266, which needed scripts for serial transfers as the IDE tools failed.
- **Solutions Implemented**: After experimentation, simpler interrupt routines and a single-byte buffer system were settled upon. This resolved many latency and crash issues.

### Matthew Komitsky's Micro Mouse Project

- **Overview**: Developing a PCB and obtaining motors in preparation for a competitive Maze-Solving Robot.
- **Technical Approach**: PCBs are designed for small scale motors with integrated encoders, with SMT soldering done manually due to prototyping small volumes.
- **Challenges**: Addressing solder bridging during PCB assembly. Developed a manual pick-and-place setup to accurately position components.
- **Future Goals**: Testing hardware as components like PCBs and motors arrive, with an aim to compete by March.

### Fernando's Iron Rain Robotics Launcher

- **Project Goal**: Creating a flywheel mechanism to launch balls efficiently for a robotics competition.
- **Issues Faced**: 
  - Wobbling of the flywheel causing instability.
  - Insufficient power and ball trajectory leading to less-than-expected distances during test launches.
- **Discussion Points**: Consideration of using dual flywheels for stability, adjusting friction material, or altering structures for enhanced power transfer and accuracy.
- **Proposed Experiments**: Testing different compression and friction scenarios, potential integration of a belt drive, or adding a secondary flywheel for balance.

### Surface Mount Device (SMD) Soldering

- **Dave Ackley’s Demonstration**: Successfully demonstrated hand soldering techniques on SMDs using tweezers and fine-tip soldering irons, emphasizing the necessity of adequate fluxing.
- **Community Insights**: Shared experiences about soldering SMDs ranging from tip selection to mitigating thermal effects during hot air gun use.

## Referenced Links

- Ponder SomeMore provided a link to Mr. Solder Fix’s YouTube Channel for soldering techniques and tips: 
  - [Mr. Solder Fix](https://www.youtube.com/@mrsolderfix3996)

These focused interactions and knowledge exchanges continue to empower members in tackling complex projects and refining their technical skills.
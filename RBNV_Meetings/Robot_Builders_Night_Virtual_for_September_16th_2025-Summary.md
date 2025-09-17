# Robot Builders Night Virtual for September 16th, 2025

## Introduction
The meeting included discussions on various robotics projects, challenges in robot navigation, the use of simulation tools, and shared resources for building and programming robots. Attendees also explored technical issues encountered during robot operations and novel solutions for improving these systems.

## Meeting Highlights

### Robot Navigation and Issues
- **Mike Williamson** discussed challenges faced with ROS 2 Navigator, particularly its issue with sending multiple and conflicting commands when near obstacles. Mike explained a temporary fix of waiting two seconds to allow commands to settle before switching navigation modes.
- He also explored a cone detection issue using LIDAR where infinity readings from edge detection created challenges in ensuring reliable distance measurements.
  
### In-Home Robot Testing
- **Douglas Paradis** shared insights from setting up an RTK (Real-Time Kinematic) system for navigation in his home. Despite environmental challenges, he achieved fixed solutions with the RTK.

### Simulation and Modeling
- **Paul Bouchier** introduced a newly acquired robot capable of running ROS 2 on an ESP32 and demonstrated its assembly and initial setup.
- **Carl Ott** introduced the MuJoCo Simulation, a physics engine used for modeling and simulating robotic dynamics.

### New Technologies and Resources
- **Paul Bouchier** showcased a "makers pet" robot, which is ROS 2 compatible and aligns with the Leno robot software stack. The ease of setup and configuration makes it suitable for beginners.
- **John K** mentioned a new open-source robot design, Mevita, aimed at being cost-effective and accessible for robot builders. 

## Conclusions and Insights
- Navigation challenges in cluttered environments remain a key issue, with potential solutions focusing on better control algorithms and enhanced sensory input.
- Use of RTK technology for precise localization shows promising results even in constrained environments but requires more robust setup for outdoor applications.
- The introduction of affordable, accessible robotic kits aids in lowering barriers to entry for new robotics enthusiasts, fostering learning and development.

## Referenced Links
- **Ponder SomeMore**
  - [Makers Pet Robot Models](https://github.com/makerspet/3d_models/tree/main/loki_200mm/stl/)
  - [Mevita Hardware Platform](https://haraduka.github.io/mevita-hardware/)

- **Carl Ott**
  - [MuJoCo Simulator](https://www.bing.com/ck/a?!&&p=2a747e85a7b6b29da4de9e3043adf94cfa4ceb1b9ee80b0d24ce343504065e7bJmltdHM9MTc1Nzk4MDgwMA&ptn=3&ver=2&hsh=4&fclid=3aef7fbf-f84c-6719-21ca-6c07f91b6696&psq=mujoco+simulation&u=a1aHR0cHM6Ly9naXRodWIuY29tL2dvb2dsZS1kZWVwbWluZC9tdWpvY28)
  - [Google DeepMind's MuJoCo on GitHub](https://github.com/google-deepmind/mujoco)
  - [MuJoCo Official Site](https://mujoco.org/)

This session provided valuable exchanges on innovative robotics technologies and practical problem-solving strategies for current robotics challenges. Participants were encouraged to further explore shared resources and discussed technologies to enhance their own projects.
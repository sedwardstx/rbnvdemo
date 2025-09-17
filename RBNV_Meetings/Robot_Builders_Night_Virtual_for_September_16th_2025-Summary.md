# Robot Builders Night Virtual for September 16th, 2025

## Video at https://youtu.be/-i8gqXXJMCE

### Robot Navigation and Issues
- **Mike Williamson** discussed challenges faced with ROS 2 Navigator, particularly its issue with sending multiple and conflicting commands when near obstacles. Mike explained a temporary fix of waiting two seconds to allow commands to settle before switching navigation modes.
- He also explored a cone detection issue using LIDAR where infinity readings from edge detection created challenges in ensuring reliable distance measurements.
  
### In-Home Robot Testing
- **Douglas Paradis** shared insights from setting up an RTK (Real-Time Kinematic) system for navigation in his home. Despite environmental challenges, he achieved fixed solutions with the RTK.

### Makerspet Ros2 robot for $150
- **Paul Bouchier** introduced a newly acquired robot capable of running ROS 2 on an ESP32 and demonstrated its assembly and initial setup.
- The "makers pet" robot aligns with the Linorobot software stack. The ease of setup and configuration makes it suitable for beginners.

### Other topics
- **John K** mentioned a new open-source robot design, Mevita, aimed at being cost-effective and accessible for robot builders. 

## Referenced Links
- **Ponder SomeMore**
  - [Makers Pet Robot Models](https://github.com/makerspet/3d_models/tree/main/loki_200mm/stl/)
  - [Mevita Hardware Platform](https://haraduka.github.io/mevita-hardware/)

- **Carl Ott**
  - [MuJoCo Simulator](https://www.bing.com/ck/a?!&&p=2a747e85a7b6b29da4de9e3043adf94cfa4ceb1b9ee80b0d24ce343504065e7bJmltdHM9MTc1Nzk4MDgwMA&ptn=3&ver=2&hsh=4&fclid=3aef7fbf-f84c-6719-21ca-6c07f91b6696&psq=mujoco+simulation&u=a1aHR0cHM6Ly9naXRodWIuY29tL2dvb2dsZS1kZWVwbWluZC9tdWpvY28)
  - [Google DeepMind's MuJoCo on GitHub](https://github.com/google-deepmind/mujoco)
  - [MuJoCo Official Site](https://mujoco.org/)


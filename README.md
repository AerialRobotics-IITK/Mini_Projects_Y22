# Mini Projects

For the **year 2023-2024**, we have decided upon five mini-projects which are aimed at specializing members in certain domains to enhance the strength of the team. We would likely keep 3/4 people in each project. All the projects would be implemented both on hardware and software.

Below is a detailed description of each of the projects:

## 1. Video Tracker & Pick-Up

### **Demo of Final Deliverable:**

<a href="https://drive.google.com/file/d/1Zbe3OWqVA89yEYJfSTbyKQV7BlBUXbkC/view" target="_blank"><img src="https://thumbs2.imgbox.com/78/07/uyLK3XzJ_t.png" alt="image host" width="350" height="200"/></a>


[](https://drive.google.com/file/d/1Zbe3OWqVA89yEYJfSTbyKQV7BlBUXbkC/view)

### Deliverables:

We would implement a **full-fledged object tracking algorithm as shown in the demo in simulation and hardware**. We would further extend it by implementing a **grid search and object-pick-up again in both simulation and hardware.**

### Concepts Involved

This project would lay heavy emphasis on image processing techniques. Further, below are short pointers on overall concepts that would be involved.

- Detection
    - Classical Methods such as thresholding & correlation
    - Machine Learning Methods (specifically, CNNs and YOLO)
    - Parallel Computing Techniques and their implementation using CUDA, laying emphasis on image processing applications
- Tracking
    - It would be a deep dive into tracking algorithms such as KCF, MOSSE, DCF, etc.
- Object Localization
- Grid Search
    - For searching for a predetermined object in a given area.
- Pick Up
    - Control of Gripper Actuators autonomously, i.e. configuring its opening/closing on certain triggers.

### Hardware Involved

The following details hardware that would be involved apart from the normal build of an autonomous drone.

Onboard Computer: **Jetson**, since we would be aiming to implement GPU acceleration using CUDA to enhance the performance of our image processing algorithms.

Camera: **RunCam**

External Hardware: Gripper

## 2. Control & SLAM

### **Demo of Final Deliverable:**

[![DEMO_SWARM](https://img.youtube.com/vi/EbzfjNpLzvg/0.jpg)](https://www.youtube.com/watch?v=EbzfjNpLzvg)

### Deliverables:

We would be first delving into design Control Theory, and **implement atleast 3 popular controller models from scratch with benchmarking**. This would be followed by learning about pose estimation techniques, including **VIO and Kalman Filters** (eg. to fuse GPS data in position estimates). Finally, we would be **implementing a SLAM module** for quadcopters and **mapping an area**. 

### Concepts Involved:

The project would heavily revolve around control theory and pose estimation techniques, since it forms a requisite knowledge for one to completely understand SLAM.

- Controllers
- GPS
- RealSense Simulation Setup using RViz
- Map Generation, SLAM

### Hardware Involved:

The following details hardware that would be involved apart from the normal build of an autonomous drone.

- Onboard Computer: **Jetson or Odroid**
- External Hardware: RTK

## 3. Swarm

### **Demo of Final Deliverable:**

[![DEMO_SWARM](https://img.youtube.com/vi/cAXUKNGpMG4/0.jpg)](https://www.youtube.com/watch?v=cAXUKNGpMG4)

### Deliverables:

As depicted in the demo video, we would implement a drone swarm, whilst adding modules for formation flying, collision avoidance. Further, we would also implement a hierarchial swarm framework, wherin slave drones follow a master drone.

### Concepts Involved:

A major chunk of the project would focus on creating the communication framework for the swarm, thus involving a lot of **networking concepts.** To ensure coordinated movement and formation flying, we would be implementing a **waypoint generation and path planning** module. 

### Hardware Involved:

We would be implementing a swarm of three drones, thus a build of three drones would be required.

- Onboard Computer: **Odroid**
- External Hardware: Router

## 4. Autonomous FPV

### Demo of Final Deliverable:

[![DEMO_FPV](https://img.youtube.com/vi/XpuRpKHp_Bk/0.jpg)](https://www.youtube.com/watch?v=XpuRpKHp_Bk)

### Deliverables:

As depicted in the demo video, we will implement an **autonomous FPV racer** using motion capture. 

### Concepts Involved:

The major chunk of the project would revolve arounding implementing optimized autonomous navigation algorithms. This would subsequently involved trajectory generation, and publishing of the generated waypoints. There will be some overlap in the aspect of control with other project based on SLAM, we would not delve into controls in much detail here.

### Hardware Involved:

The following details hardware that would be involved apart from the normal build of an autonomous drone.

- Onboard Computer: **Raspi or Odroid**
- Camera: RunCam
- External Hardware: Gimbal

## 5. Hardware Exploration

### Deliverables:

It will be expected that at the end of this project, you will be capable of assemble a complete build of drone, proficiency in manually flying the drone as well as running missions on the drone. The members will also be expected run any repository and implement it quickly. This subgroup will also be responsible for preparing the hardware for the all the other mini-projects. They should also be able to choose the appropriate hardware for any problem statement.

### Concepts / Ideas Involved:

Quickly assembling a drone and preparing it for the mission is critical for ensuring that the software stack is tested as soon as it is ready, which will go a great deal in ensuring success in any competition. Debugging is essential here as it is not always easy to download dependencies onto the onboard computer. 

Ardupilot, the firmware going to be used, is complex has a lot of parameters to be fine-tuned, and problems are difficult to pinpoint if one isn’t well versed with its vast documentation. Finally, a team without any flyers is not a aerial team. Thus, we need people willing to spend the hours to master flying, which is also essentially, when a mission doesn’t go as planned.

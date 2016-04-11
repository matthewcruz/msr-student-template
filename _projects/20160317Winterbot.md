---
layout: project
title: '6 DOF Robot Arm'
date: March 2016
image: '/portfolio/public/images/gripper.JPG'
---

## Overview
"Winterbot" is a six degree of freedom (DOF) robot arm with a custom designed gripper that was developed and built during winter quarter for the Masters in Robotics at Northwestern University.
The design uses 7 dynamixel servos (6 for the arm and one for the gripper) to get a full range of motion in 3-D space. The servos are controlled via MoveIt! in ROS that interfaces with a robot microcrontroller through serial connection.  The robot can be controlled via the RVIZ gui or a a script that controls an interactive marker using a Sony PS3 Joystick controller.

<img src="/portfolio/public/images/arm.png" width="640" heigth="320"/>

### Current Work
Current work is being done to optimize arm control with an analytic Inverse Kinematics solver to  in order to control the position of the robot's end effector more efficiently and in near real-time. 

### Follow the link below to see a sample video
 
### <a href="https://youtu.be/KL_vttfEQBo">"Winterbot" controlled through MoveIt! to Record and Playback waypoints</a>


 <!--video width="640" height="480">
    <source src="https://youtu.be/zu6un1K--iY" type="video/mp4"/>
    <source src="https://youtu.be/zu6un1K--iY" type="video/ogg"/>
</video-->


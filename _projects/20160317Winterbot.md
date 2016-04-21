---
layout: project
title: '6 DOF Robot Arm'
date: March 2016
image: '/portfolio/public/images/gripper.JPG'
---

## Overview
"Winterbot" is a six degree of freedom (DOF) robot arm with a custom designed gripper that was designed and built during winter quarter for the Masters in Robotics at Northwestern University.
The design uses 7 dynamixel servos (6 for the arm and one for the gripper) to get a full range of motion in 3-D space. The servos are controlled through ROS (optionally through MoveIt!) that interface with a robot microcrontroller through serial connection.  The robot can be controlled via the RVIZ gui or a script that controls an interactive marker using a Sony PS3 Joystick controller.

<img src="/portfolio/public/images/arm.png" width="640" heigth="320"/>

### Current Work
Current work is being done to optimize arm control with an analytic Inverse Kinematics solver and custom planner to control end-effector position more efficiently in near real-time. Additionally, vision is being integrated to allow for pick-and-place operations in 3D space.

The following video shows communication of Winterbot with MoveIt! by visualizing the joint states live on the RVIZ interface. First, the robot is relaxed through a service call to each servo to allow for manual manipulation. Then the robot is placed in poses and the encoder values are saved. Upon execution, MoveIt! shows the planned path and executes the trajectory motion to each saved waypoint. At the end of the video, gripper control is demonstrated with a board marker.

<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/KL_vttfEQBo" frameborder="0" allowfullscreen></iframe></p>



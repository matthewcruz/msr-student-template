---
layout: project
title: '6 DOF Robot Arm'
date: March 2016
image: '/portfolio/public/images/gripper.JPG'
---

## Overview
"Winterbot" is a six degree of freedom (DOF) robot arm with a custom designed gripper that was designed and built during winter quarter for the Masters in Robotics at Northwestern Univeristy.
The design uses dynamixel 7 dynamixel servos (6 for the arm and one for the gripper) to get a full range of motion in 3-D space. The servos are controlled via MoveIt! in ROS that interfaces with a robot microcrontroller through serial connection. 

<img src="/portfolio/public/images/arm.png" width="640" heigth="320"/>

Current work is being done to integrate the arm with an analytic Inverse Kinematics solver to interpret Sony PS3 joystick commands in order to control the position of the robot's end effector. 

 <video width="640" height="480">
    <source src="https://youtu.be/zu6un1K--iY" type="video/mp4"/>
    <source src="https://youtu.be/zu6un1K--iY" type="video/ogg"/>
</video>


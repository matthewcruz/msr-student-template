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


After designing the main joystick controller interface, I created a planner that performs "uninformed" local search to move to its goal location in space. The following pictures demonstrate the moveit planner(RRTstark from OMPL) on the Left and a graph of my real-timeplanner on the right.<br>
<img src="/portfolio/public/images/moveit_traj.png" style="background-color:white;" height="250"/>
<img src="/portfolio/public/images/planner1.png" style="background-color:white;" height="250"/>

### Moving Forward

I would like to create a weighted policy or cost function that takes the previously explored task space and creates pathways for least energy for each location. The idea would be to thoroughly explore the task space and provide a simplified and weighted computation to move from one position to another given an unknown command from the user. This planner would incorporate knowledge of joint limits and self-collision areas into the policy/cost-function.

### Example

The following video shows communication of Winterbot with MoveIt! by visualizing the joint states live on the RVIZ interface. First, the robot is relaxed through a service call to each servo to allow for manual manipulation. Then the robot is placed in poses and the encoder values are saved. Upon execution, MoveIt! shows the planned path and executes the trajectory motion to each saved waypoint. At the end of the video, gripper control is demonstrated with a board marker.

<p align="center">
<iframe width="560" height="315" src="https://www.youtube.com/embed/KL_vttfEQBo" frameborder="0" allowfullscreen></iframe></p>



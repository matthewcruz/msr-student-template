---
layout: project
title: 'Quadcopter Design'
date: June 2016
image: '/portfolio/public/images/quad.JPG'
background: 

---

### Overview
During the "Quadcopter" project course taught by Professor Mike Rubenstein, myself and a colleague assembled and programmed a joystick-controlled quadcopter. We programmed the motion control from the ground up in C to be ran on a Rasberry Pi.

### Control
To control the quadcopter an Inertial Measurement Unit (IMU) mounted on the assembled quadcopter was used to gather gyroscopic and linear acceleration measurements. These measurements were queried from the IMU via the I2C communication protocol. A complimentary filter merged drift-prone gyroscope values with noisy accelerometer values to yield low long-term drift and less noise-prone roll and pitch rates, which were integrated for orientation in degrees. To control the heading of the quadcopter, PID control was implemented on the orientation values for roll and pitch. Final control of orientation was achieved through a PWM breakout board connected to the four Electronic Speed Controllers (ESC) of the quadcopter motors.  

In addition to basic motion control, controls were added for orientation calibration, yaw velocity, thrust, safety cutoffs (in the case of communication loss/timeout, extreme angles or "yaw" over-speed).

### Communication
In order to control the quadcopter in real-time a server script was run on a linux system which conveyed joystick commands to a client scipt running on the Rasberry Pi. The linux system and Rasberry Pi were then networked over Wifi. 

<!--img src="/portfolio/public/images/quad.JPG" align="MIDDLE" width="640" heigth="320"/-->

<!--image: '/portfolio/public/images/quad.JPG'-->





---
layout: project
title: 'Quadcopter'
date: June 2016
image: '/portfolio/public/images/quad.JPG'
---

## Overview
During this project myself and a colleague assembled and programmed a Joystick-Controlled quadcopter.

#Communication
In order to control the quadcopter in real-time a server script ran on a linux system connecting joystick commands with a client scipt running on the Pi. The linux system and Pi were then networked over Wifi. 

#Control
Rotational speeds and linear accelerations were queried from the IMU via I2C.
A complimentary filter merged drift-prone gyroscope values with noisy accelerometer values with a compilation filter to yield low long-term drift and less noise-prone roll and pitch rates, which were integrated for orientation in degrees. PID control was implemented on the orientation values for Roll and Pitch. Final control of orientation was achieved through a PWM breakout board communicating over I2C to four Electronic Speed Controllers (ESC), one for each motor.  

In terms of functionality, controls were added for orientation calibration, yaw velocity, thrust, safety cutoffs(loss of communication/timeout errors) for extreme-angles and yaw "over-speed".

<img src="/portfolio/public/images/quad.JPG" width="640" heigth="320"/>





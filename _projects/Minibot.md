---
layout: project
title: Current Projects
date: 2017-01-01
image: '/portfolio/public/images/internals.JPG'
background: '/portfolio/public/images/green-aurora-clouds.jpg'
font: white
---


## Overview
I am happy to say that I have begun a NEW PROJECT to use both Robotics and mechanical design.
I am making a miniature humanoid robot, which I have not-so-codenamed "Minibot".

The idea behind this little guy was to combine alot of different skills into one, big-bad standalone project, and along the way pick up some new ones. I will try to document my work as it comes along.

## Goals
The main goals of this project are:
<br>
1. Aesthetic - The body should be organic and made through surface modelling <br>
2. Functional - The robot should have some nice functionality that hasn't been see too much <br>
3. Autonomous - The robot should be somewhat responsive to external stimuli other than commands <br>
4. Fun - I would like to bring some interesting moves and functionality

## Current Plan
So since this is a humanoid I have designed it to have two arms, a torso, some kind of head, and other than that... I'm still planning.
So far I have planned three DOF arms, a tft touchscreen (about 2.2") for the head, a camera (720p) in the chest, face and, possibly, object recognition - and depending on the platform - voice recognition (Which should really step this project up). 

The "depending on the platform" means that I am trying to decide between the new Raspberry Pi Zero-W which offers alot of functionality in 2"x1" package.... or....use a really fast microcontroller like the Atmel SAM s70/e70 series (300 MHz) so I can do some rudimentary image processing. I have currently built some Image processing libraries from the ground up using Python, and have also used the OpenCV complements. This makes it easy to use the Raspberry Pi and pi camera with the onboard port, but I would like to try my hand at programming the libraries in C (maybe too much to take on).

As for the motion control, I will be using a small microcontroller (like the arduino uno or clone), and driving motion profiles and kinematics from there (I've written the libraries for PID's, motion profiles and FK/IK for these). A serial interface is all i need then to send primitive commands and get back status. 

## Status Updates

### April 4th 2017
So far I have finished the surface modelling of the arms, finalized the joints, and designed the mechanical and mechatronics for the arms. I havent quite finished the torso, so that will be coming a little later. But below I have included pictures of the industrial design of the arms, a CAD model of the internal mechanism and the first prototype. 

<img src="/portfolio/public/images/armAssyPrint.JPG" width="320" heigth="320"/>
<img src="/portfolio/public/images/upperArmCAD.PNG" width="320" heigth="320"/>
<img src="/portfolio/public/images/internals.JPG" width="640" heigth="320"/>

Background image credit: skyandtelescope.com


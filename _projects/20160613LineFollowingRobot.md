---
layout: project
title: 'Line Following Robot'
date: June 2016
image: '/portfolio/public/images/final_pcb.JPG'

---

### Overview
A line following robot was designed and built to compete in a term competition for the Advanced Mechatronics class at Northwestern University. This term project required the design and fabrication of a visual processing system, motor control system and a chassis. 

The robot design consisted of the following main components:

<body>
    <ul>
    <li>Android application running on an Android phone with integral camera</li>
    <li>Custom PCB (PIC32)</li> 
    <li>Themed chassis design and assembly (Laser-cut and 3D printed)</li>
    </ul>
</body>

<img src="/portfolio/public/images/app.JPG" align="MIDDLE" width="320" heigth="320"/>


### Android App
The Android phone was designed to use the integral camera to capture continuous images of the track. These images were processed by the phone using color filtration to distinguish the path line from the background. The phone then sent a control signal via USB-serial (cdc) to the microcontroller (PIC 32) on the custom designed PCB.

<figure>
    <img src="/portfolio/public/images/breadboard.JPG" align="MIDDLE" width="350" heigth="640"/>
</figure>

### PCB Design
The PIC32-based breadboard was designed to control the robot. A picture of the breadboard is shown above. Following proof of concept, the board schematic was drawn in Eagle CAD software and sent to a production house to be manufactured. The schematic and final board example are shown below. The code to control the PCB was written using a cdc-serial enumerator integrated from the Harmony library. This allowed communication with the Android phone. The signal sent by the phone was converted into a control signal that was fed into a a PID loop and issued to the two motors of the differential drive robot through a dual H-bridge. 

<img src="/portfolio/public/images/board.png" align="MIDDLE"  width="280"/>
<img src="/portfolio/public/images/final_pcb.JPG" align="MIDDLE" width="320" heigth="640"/>


### Chassis Design
The Chassis was designed to be laser cut and utilized a crenellation for interlocking planar pieces that created a 3D structure. Motor mounts, and wheels were 3D printed to complete the design. A little personal touch was added to the asthetic design.

<img src="/portfolio/public/images/chassis.JPG" align="MIDDLE" width="640" heigth="640"/>


### Videos of the working robot
<iframe width="560" height="315" src="https://www.youtube.com/embed/w2bhnCp7T6M" frameborder="0" allowfullscreen></iframe>


<iframe width="560" height="315" src="https://www.youtube.com/embed/fup4hfyTwDg" frameborder="0" allowfullscreen></iframe>





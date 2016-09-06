---
layout: project
title: 'Line Following Robot'
date: June 2016
image: '/portfolio/public/images/final_pcb.JPG'

---

###Overview
A line following robot was designed and built to compete in a term competition for the Advanced Mechatronics class at Northwestern University. This term project required the design and fabrication of a visual processing system, motor control system and a chassis. 

The robot design therefore consisted of the following main components:

<body>
    <ul>
    <li>Android Application running on an Android Phone with Integral Camera</li>
    <li>PCB breadboard, CAD design and Assembly</li> 
    <li>Chassis design and Aseembly using Laser-cutting and 3D printing</li>
    </ul>
</body>

<img src="/portfolio/public/images/app.JPG" align="MIDDLE" width="320" heigth="320"/>


###Android App
The Android phone was designed to use the integral camera to capture continuous images of the track. These images were processed by the phone using color filtration to distinguish the path line from the background. The phone then sent a control signal via USB-serial (cdc) to the microcontroller (PIC 32) on the custom designed PCB.

<figure>
    <img src="/portfolio/public/images/breadboard.JPG" align="MIDDLE" width="350" heigth="640"/>
</figure>

###PCB Design
The PCB breadboard of the original PCB is shown to the right with all peripherals on-board. Once the circuit design was built, the schematic was drawn digitally in Eagle CAD software and sent to a production house for manufacture.The code to control the PCB was written using a cdc-serial enumerator integrated from the Harmony library. This allowed communication with the Android phone. The signal recieved was then converted into a control that was fed into a a PID loop and issued to the two motors of the differential drive robot through a dual H-bridge. 

<img src="/portfolio/public/images/board.png" align="MIDDLE"  width="280"/>
<img src="/portfolio/public/images/final_pcb.JPG" align="MIDDLE" width="320" heigth="640"/>


###Chassis Design

The Chassis was designed to be laser cut and utilized a crenellation for interlocking planar pieces that created a 3D structure. Motor mounts, and wheels were 3D printed to complete the design.

<img src="/portfolio/public/images/chassis.JPG" align="MIDDLE" width="640" heigth="640"/>


<iframe width="560" height="315" src="https://www.youtube.com/embed/w2bhnCp7T6M" frameborder="0" allowfullscreen></iframe>


<iframe width="560" height="315" src="https://www.youtube.com/embed/fup4hfyTwDg" frameborder="0" allowfullscreen></iframe>





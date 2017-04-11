---
layout: project
title: BLOG! Current Projects
date: March 2017
image: '/portfolio/public/images/upperArmCAD.PNG'
background: '/portfolio/public/images/green-aurora-clouds.jpg'
font: white
---
## Overview

I'm making a miniature humanoid robot! And I have not-so-codenamed it "Minibot".
The inspiration for this little guy, which will stand about 7 inches tall,  was to combine a whole lot of skills into one project, and learn as much as I can along the way.

## Goals

<style>
	ul { list-style-type:none;}
</style>
The main goals of this project are: <br><br>
<b><u> Aesthetic</u> </b>- Organic body curves (eliminate servo form factor) <br>
<b><u> Functional</u> </b>- Create utility AND a personality through function <br>
<b><u> Autonomous and Fun</u> </b> - Because these two tend to go together in my mind ...Minibot will be (somewhat) responsive to external stimuli without needing direct commands ... and although this project started before I heard about <a href="https://anki.com/en-us/cozmo" target="_blank">Cozmo </a>, by Anki, I was nonetheless inspired to incorporate the spirit of a learning robot that is fun to interact with.<br>
<b><u> Mini</u> </b> - I want the challenge of making this robot small... packing alot of power in a fun-size humanoid

## Current Plan
So far I have planned three DOF arms, a tft touchscreen (about 2.2") for the head, a camera (720p) in the chest, face recognition (and possibly Object recognition). And, <b><i>  depending on the platform</i> </b>, voice recognition (Which should really step this project up). 

<ul>
	<li>
<b><i> Microcontroller or Microprocessor? </i> </b> <br>
A choice that determines code flexibility, access to open-source libs, speed, hardware peripherals etc. I have the Raspberry Pi Zero-W  on one hand (with a 2"x1" package, <b>1 GHz proc. </b>, dedicated cam port, access to: OpenCV, PocketSphynx, and my Python libs... And on the other hand something like Atmel SAM s70/e70, clocking at 300 MHz, lightweight, pushing me to transfer alot of my libs to C and create fast image processing code -Think <a href="http://www.cmucam.org/" target="_blank">Pixy CMUcam5</a>- (i don't know if that's good or bad)... <br> </li>
<li>
	<br>
<b><i> Modular </i> </b> <br>
A smaller scale microcontroller like <b> <i> Arduino uno  </i> </b>will do low level motion control profiles, adaptive PID's, and possibly kinematics, communicating with the main brain via serial with simple state machine controls. </li>
</ul>

## Status Updates

### April 10th 2017
It's working .... almost. Some small mistakes in CAD led to a reprint of the Upper arm ( a small battle because of the support material settings of the 3D printer). But even after a nice print, I found that the smaller features needed for alignment were not coming out, So I made some alignment tools to really get the detail I needed for the gears to mesh. Then I made a test bed using an Aruduino Uno driving a low voltage <b> Pololu</b> motor carrier, A potentiometer whose signal runs through an analog multiplexer (for when I have alot of motors), feeeding into the ADC on the arduino to control PWM duty cycle (motor speed). Here is the arm half assembled for testing and the test bed!
<li>
		<img src="/portfolio/public/images/parts_loose.JPG" width="200" heigth="200" alt="parts_loose" usemap="#parts_loose"/>
		<map name= 	"parts_loose">
		<area shape="rect" coords="0,0,200,200" alt="parts_loose" href= "/portfolio/public/images/parts_loose.JPG" target = "_blank">
		</map>
		<img src="/portfolio/public/images/upper_angled.JPG" width="200" heigth="200" alt="upper_angled" usemap="#upper_angled"/>
		<map name= 	"upper_angled">
		<area shape="rect" coords="0,0,200,200" alt="upper_angled" href= "/portfolio/public/images/upper_angled.JPG" target = "_blank">
		</map>
		<img src="/portfolio/public/images/upper_be.JPG" width="200" heigth="200" alt="upper_be" usemap="#upper_be"/>
		<map name= 	"upper_be">
		<area shape="rect" coords="0,0,200,200" alt="upper_be" href= "/portfolio/public/images/upper_be.JPG" target = "_blank">
		</map>
		<img src="/portfolio/public/images/test_setup.JPG" width="200" heigth="200" alt="test_setup" usemap="#test_setup"/>
		<map name= 	"test_setup">
		<area shape="rect" coords="0,0,200,200" alt="test_setup" href= "/portfolio/public/images/test_setup.JPG" target = "_blank">
		</map>

</li>


<b>Lessons Learned: </b>
<ol>
	<li> <b> Printer setting make a difference</b></li>
		I knew the holes I printed would not be exact as the 0.1mm tolerances I needed, so I had to create some helpful tools. The first was a <i> "Hole chart" </i>, which has holes in 0.1 mm increments acting as a "plug-gaged" for the 1.0mm and 1.5mm shafts I was using. This gave me an idea of how to size my printed part. 
	<li> <b> Assembly tools are your friend </b></li>
		Again, tolerances make a big difference with 0.3 module gears!! Pitch diameters have to line up! And printing holes into the structure just wouldn't do. In step a manufacturing tool and the right drill bits. I printed this assembly fixture using what i learned from the hole chart to get a nice press fit size hole, and made it nice and tall to act as a guide(at least 3x the drill bit diam.) I used this to repeatablly and accurate drill in the shaft holes for the gears to get "perfect" meshing! The second is a similar fixture to drill a a 1.4-1.5mm hole into the gear with a 0.9mm hole.<br>
		<img src="/portfolio/public/images/jigs.JPG" width="200" heigth="200" alt="jigs" usemap="#jigs"/>
		<map name= 	"jigs">
		<area shape="rect" coords="0,0,200,200" alt="jigs" href= "/portfolio/public/images/jigs.JPG" target = "_blank">
		</map>
		<img src="/portfolio/public/images/jig_assy.JPG" width="200" heigth="200" alt="jig_assy" usemap="#jig_assy"/>
		<map name= 	"jig_assy">
		<area shape="rect" coords="0,0,200,200" alt="jig_assy" href= "/portfolio/public/images/jig_assy.JPG" target = "_blank">
		</map>
	<li> <b>Slop ... its Good and Bad </b></li>
		If you have tight tolerance you get exact alignment, if they are too tight, small imperfections will bind you up! And so, I need to develop a little plate that will keep the shafts inline relative to eachother during assembly. Luckily This isn't too hard :). But I may need to float the motor with an oring or rubber gasket to allow some play in case of runout on the gear shaft. And kind of unrelated, but expected, the o-ring needs to be a harder durometer. Harder durometer = less stretch and less inaccruacy when driving the pulley. 
</ol>


### April 4th 2017
So far I have finished the first round of surface modelling of the arms.
I have designed out the mechanics of the upper arm and am trying to fit the mechanics into the lower arm. I havent quite finished the torso, so that will be coming a little later. But below I have included pictures of the industrial design of the arms, a CAD model of the internal mechanism and the first prototype. <br>
<!-- https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_areamap --> <b> Click on Images to Enlarge! </b> <br><br>
<li>
<img src="/portfolio/public/images/armAssyPrint.JPG" width="200" heigth="200" alt="armAssy" usemap="#armAssyPrint"/>
<map name= 	"armAssyPrint">
<area shape="rect" coords="0,0,200,200" alt="armAssy" href= "/portfolio/public/images/armAssyPrint.JPG" target = "_blank">
</map>


<img src="/portfolio/public/images/upperArmCAD.PNG" width="200"  alt="upperArmCAD" usemap="#upperArmCAD" />
<map name= 	"upperArmCAD">
<area shape="rect" coords="0,0,200,200" alt="armAssy" href="/portfolio/public/images/upperArmCAD.PNG" target = "_blank">
</map>

<img src="/portfolio/public/images/internals.JPG" width="200" alt="internals" usemap="#internals" />

<map name= 	"internals">
<area shape="rect" coords="0,0,200,200" alt="armAssy" href="/portfolio/public/images/internals.JPG" target = "_blank">
</map>
</li>

Background image credit: skyandtelescope.com


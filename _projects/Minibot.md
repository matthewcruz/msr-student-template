---
layout: project
title: BLOG! Current Projects
date: March 2017
image: '/portfolio/public/images/upperArmCAD.PNG'
background: '/portfolio/public/images/green-aurora-clouds.jpg'
font: white
---
## Overview

I'm making a miniature humanoid robot which I have not-so-codenamed "Minibot"!!
The inspiration for this little guy, which will stand about 7 inches tall,  was to combine all of the mechanical, design, robotics and embedded design skills i have acquired into one project, and learn as much as I can along the way.

## Goals

<style>
	ul { list-style-type:none;}
</style>
The main goals of this project are: <br><br>
<b><u> Aesthetic</u> </b>- Have soft organic body curves (eliminate servo form factor) <br>
<b><u> Functional</u> </b>- Create utility AND a personality through function <br>
<b><u> Autonomous and Fun</u> </b> - Because these two tend to go together in my mind ...Minibot will be (somewhat) responsive to external stimuli without needing direct commands ... and although this project started before I heard about <a href="https://anki.com/en-us/cozmo" target="_blank">Cozmo </a>, by Anki, I was nonetheless inspired to incorporate the spirit of a learning robot that is fun to interact with.<br>
<b><u> Mini</u> </b> - I want the challenge of making this robot small... packing alot of power in a fun-size humanoid

## Current Plan
So far I have planned three DOF arms, a tft touchscreen (about 2.2") for the head, a camera (720p) in the chest, face recognition (and possibly Object recognition). And, <b><i>  depending on the platform</i> </b>, voice recognition (Which should really step this project up). 

<ul>
	<li>
<b><i> Microcontroller or Microprocessor? </i> </b> <br>
A choice that will decide alot for this project (i.e. code flexibility, access to open-source libs, speed, hardware peripherals etc.) On one hand I can go the single board computer route such as the Raspberry Pi Zero-W (with a 2"x1" package, <b>1 GHz single core proc. </b>, dedicated cam port, access to: OpenCV, PocketSphynx, and my Python libs... And on the other hand i could implement a microcontroller like Atmel SAM s70/e70, clocking at 300 MHz, lightweight, pushing me to transfer alot of my libs to C and create fast image processing code (i don't know if that's good or bad, but a challenge for sure)-Think <a href="http://www.cmucam.org/" target="_blank">Pixy CMUcam5</a>- but with no coprocessor ... <br> </li>
<li>
	<br>
<b><i> Modular </i> </b> <br>
The design will be broken intro modules, where a microcontroller like <b> <i> Arduino uno  </i> </b>will perform low level motion control profiles, adaptive PID's, and possibly kinematics, communicating with the main brain processor via serial with simple state machine controls. </li>
</ul>
<hr>
## Status Updates

### April 14th 2017
<ul>
<li>
This week was so satisfying. I was able to print the first couple prototypes after CADing the upper arm, tweaking the mechanics just right to get them to fit, waiting on parts to ship from HongKong/everywhere and reCADing to fix some small errors. And as of April 10th I have a it.. pretty much running. Even better, I was able to test out most of the design flaws! 
As I wrapped up the upper Arm, I finally got the CAD done on the lower arm. This really took alot of doing because the mechanics were so hard to fit. I ultimately ended up widening the forearm/lower arm. I still have some minor adjustments to do to make sure all the tolerances are right for the print, but the bulk of the work on the arm is DONE!
<br> <b> Click to Enlarge! </b> <br><br>

		<img src="/portfolio/public/images/arm_assy_iso.png" style="background-color:white;" width="300" heigth="300" alt="arm_assy_iso" usemap="#arm_assy_iso"/>
		<map name= 	"arm_assy_iso">
		<area shape="rect" coords="0,0,300,300" alt="arm_assy_iso" href= "/portfolio/public/images/arm_assy_iso.png" target = "_blank">
		</map>
		<img src="/portfolio/public/images/arm_assy_land.png" style="background-color:white;"  width="300" heigth="300" alt="arm_assy_land" usemap="#arm_assy_land"/>
		<map name= 	"arm_assy_land">
		<area shape="rect" coords="0,0,300,300" alt="arm_assy_land" href= "/portfolio/public/images/arm_assy_land.png" target = "_blank">
		</map>
		 
<br><br> <b> Going Forward ...</b><br> I will be printing the lower arm and then hopefully get the motion tests done for the the entire arm assembly.<br> 
<br><b> TODO</b><br>


While I'm waiting for parts to get in and time on the printer I will be getting into the motion controls. I will be transferring my libraries over from python to C so they can be run on the microcontroller. This will include: quintic and cubic motion profiles, a PID, adaptive PID and spi comm. script I already have in C, and possibly some linear algebra libraries. I will also be printing some prototypes to check out the form of the torso.<br>
<br>

<b>A little further down the road...</b><br>
I got the raspberri pi camera (v2) in today and will be playing around with that. I will also probably buy another camera to compare the performance and timing of serial vs. parallel cameras. <a href="https://www.adafruit.com/product/1386?gclid=CMqG3YX2pdMCFRiewAodYikNSg" target="_blank">These </a> adafruit ttl cameras have some interesting features... but I would really like a parallel version for speed. Also, I will be ordering the pi zero W to see how the form factor works when I print the torso. And finally I will be ordering a ~2.2" tft screen to run a simple gui using QT, Tk or something similar (don't know yet if resistive or capacitive is better - but i'm leaning towards capacitive). Until next time.  


</li>
</ul>



### April 10th 2017
<ul>
It's working .... almost. Some small mistakes in CAD led to a reprint of the Upper arm ( a small battle because of the support material settings of the 3D printer). But my second print of the upper arm is nearly functional (after a couple small hurdles of course)! However during the print I found that the smaller features needed for alignment didn't come out so well. As a result, i refined my manufacturing method and made some alignment tools to really get the detail I needed for the gears to mesh. To test the assembly and motor capabilities (torque/speed) I made a test bed using an Aruduino Uno powering the motor through a 3.3V powered <b> Pololu</b> motor carrier. A potentiometer is used for speed control, whose signal runs through an analog multiplexer (for when I have alot of motors). The analog pot. signal feeds into the ADC on the Arduino to control PWM duty cycle (motor speed). I have included pictures of the upper arm half-assembled and the test bed.
<br> <b> Click on Images to Enlarge! </b> <br>
</ul>
<ul>
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
</ul>


<b>Lessons Learned: </b>
<ol>
	<li> <b> Printer settings make a difference</b><br>
		I knew the printer couldn't get exact holes sizes down to the 0.1mm tolerances I wanted, so I had to create some helpful tools. Also, support material is .... it's just support material, its not exact and will definitely not give you the "z" dimensions you are looking for, so i ended up doing a decent share of sanding/filing.</li><br>
	<li> <b> Assembly tools are your friend </b>
		Again, tolerances make a big difference when lining up pitch diameters of 0.3 module gears!! And printing holes that need to be exact on a printer that can't print features that small makes for a little bit of work. But with the right tools, you're golden. 
		<br> To get exact holes at the right position I first created a <i> "Hole chart" </i>, which has holes in 0.1 mm increments. This showed me what fits to expect (i.e. 1.3mm designed holes printed to 1.0mm press fit). Once I know my printer, I created a machining fixture that was the negative of the arm, and lined up with the larger features. I made it nice and tall and used exact drill bits to repeatably and accuratly drill in the shaft holes for the gears.I used this same technique to bore out one of my gears from 0.9mm to 1.5mm. Success!</li> <br>
		
<br> <b> Check out the Machining fixtures below (Click to enlarge pictures)</b><br>
		<img src="/portfolio/public/images/jigs.JPG" width="200" heigth="200" alt="jigs" usemap="#jigs"/>
		<map name= 	"jigs">
		<area shape="rect" coords="0,0,200,200" alt="jigs" href= "/portfolio/public/images/jigs.JPG" target = "_blank">
		</map>
		<img src="/portfolio/public/images/jig_assy.JPG" width="200" heigth="200" alt="jig_assy" usemap="#jig_assy"/>
		<map name= 	"jig_assy">
		<area shape="rect" coords="0,0,200,200" alt="jig_assy" href= "/portfolio/public/images/jig_assy.JPG" target = "_blank">
		</map><br>
	<br><li> <b>Slop ... its Good and Bad </b></li>
		If you have tight tolerance you get exact alignment, but if too tight, small imperfections will bind you up! And so, for the next round of prototypes, I need to develop a little plate that will keep the shafts inline relative to eachother during assembly. Luckily This isn't too hard :). But I may need to float the motor with an oring or rubber gasket to allow some play in case of runout on the gear shaft. 
</ol>


### April 4th 2017
<ul>
So far I have finished the first round of surface modelling of the arms.
I have designed out the mechanics of the upper arm and am trying to fit the mechanics into the lower arm. I havent quite finished the torso, so that will be coming a little later. But below I have included pictures of the industrial design of the arms, a CAD model of the internal mechanism and the first prototype. <br>
<!-- https://www.w3schools.com/tags/tryit.asp?filename=tryhtml_areamap --> <b> Click on Images to Enlarge! </b> <br><br>
</ul>
<ul>
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
</ul>

Background image credit: skyandtelescope.com


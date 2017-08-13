---
layout: project
title: BLOG! Current Projects
date: March 2017
image: '/portfolio/public/images/full_assembly_11.png'
background: '/portfolio/public/images/green-aurora-clouds.jpg'
font: white
---
 <link rel="stylesheet" href="//code.jquery.com/ui/1.10.4/themes/smoothness/jquery-ui.css">
   <script src="//code.jquery.com/jquery-1.10.2.js"></script>
   <script src="//code.jquery.com/ui/1.10.4/jquery-ui.js"></script>
  
 <script>
   $(function() {
     $( ".accordion" ).accordion();
     $(".accordion").accordion({ header: "h3", collapsible: true, active: false ,heightStyle: "content" });
   });
   </script>


## Overview

I'm making a miniature humanoid robot and here is a little blog to document my progress.

The inspiration for this little guy, which will stand about 7 inches tall,  was to combine all of the mechanical, design, robotics and embedded design skills i have acquired into one project, and learn as much as I can along the way.

## Goals

<style>
	ul { list-style-type:none;}
</style>
The main goals of this project are: <br>
<ol>
<li><b><u> Aesthetic</u> </b> - Have soft organic body curves (eliminate servo form factor) <br></li>
<li><b><u> Functional</u> </b>- Create utility AND a personality through function <br></li>
<li><b><u> Autonomous and Fun</u> </b> - Because these two tend to go together in my mind ...Minibot will be (somewhat) responsive to external stimuli without needing direct commands<br></li>
<li><b><u> Mini</u> </b> - I want the challenge of making this robot small... packing alot of power in a fun-size humanoid </li>
</ol>

## Current Plan
(As of May  3rd 2017)<br>
The robot will comprise of a humanoid body with three degree of freedom arms, a camera, a tft touchscreen interface and voice and facial recognition. Leg's? Not sure yet, but i know that could be a nice challenge to take on... eventually.

<ul>
	<li>
<b><i> Microcontroller or Microprocessor? </i> </b> <br>
I previously had written about my decision on whether to use a microcontroller or a single board computer.
My mind is made up! Raspberry Pi zero W it is! With all manner of serial interfaces, UART, built in camera port, fast processor and wireless connectivity built in just makes this project super powerful. </li> 
<li>
	<br>
<b><i> Modular </i> </b> <br>
The design will be broken intro modules, where a microcontroller will perform low level motion control profiles, adaptive PID's, and possibly kinematics, communicating with the main brain processor via serial with simple state machine controls. </li>
</ul>
<hr>

## Status Updates

<img src="/portfolio/public/images/full_assy_torso.png"  width="100" />
 <div class="accordion">
 <h3> August 13th 2017</h3>  
     <div>
       <p><ul>
<li>
It's been more than 3 months since I've updated my progress. I recently started a new job and so things have been pretty busy. But I thought i'd add a little of the work that I forgot to add before my <i>"sabbatical"</i>. Enjoy the pictures. <br>

<br> <b> Click to Enlarge! </b> <br><br>
		<img src="/portfolio/public/images/full_assy_torso.png" style="background-color:white;" width="200" heigth="300" alt="full_assy_torso" usemap="#full_assy_torso"/>
		<map name= 	"full_assy_torso">
		<area shape="rect" coords="0,0,300,300" alt="full_assy_torso" href= "/portfolio/public/images/full_assy_torso.png" target = "_blank">
		</map>
		<img src="/portfolio/public/images/full_assy_wireframe.PNG" style="background-color:white;" width="200" heigth="300" alt="full_assy_wireframe" usemap="#full_assy_wireframe"/>
		<map name= 	"full_assy_wireframe">
		<area shape="rect" coords="0,0,300,300" alt="full_assy_wireframe" href= "/portfolio/public/images/full_assy_wireframe.PNG" target = "_blank">
		</map>

		<br> <br>

		until next time...





</li>
</ul>
</p>
     </div>
 </div>

 <div class="accordion">
 <h3> May 3rd 2017</h3>  
     <div>
       <p><ul>
<li>
It's been awhile since I've updated my progress. But I am happy to say I've made some good strides on the software front and finalized some choices on the direction. <br>

Also, check out the rendering of the Torso with Arms and the first print in low res!!!
<br> <b> Click to Enlarge! </b> <br><br>
		<img src="/portfolio/public/images/full_assembly_7.png" style="background-color:white;" width="200" heigth="300" alt="full_assembly_7" usemap="#full_assembly_7"/>
		<map name= 	"full_assembly_7">
		<area shape="rect" coords="0,0,300,300" alt="full_assembly_7" href= "/portfolio/public/images/full_assembly_7.png" target = "_blank">
		</map>
		<img src="/portfolio/public/images/full_assembly_8.png" style="background-color:white;" width="200" heigth="300" alt="fa8" usemap="#full_assembly_8"/>
		<map name= 	"full_assembly_8">
		<area shape="rect" coords="0,0,300,300" alt="fa8" href= "/portfolio/public/images/full_assembly_8.png" target = "_blank">
		</map>
		<img src="/portfolio/public/images/full_assembly_10.png" style="background-color:white;" width="200" heigth="300" alt="fa10" usemap="#full_assembly_10"/>
		<map name= 	"full_assembly_10">
		<area shape="rect" coords="0,0,300,300" alt="fa10" href= "/portfolio/public/images/full_assembly_10.png" target = "_blank">
		</map>
		<img src="/portfolio/public/images/full_assembly_11.png" style="background-color:white;" width="200" heigth="300" alt="fa11" usemap="#full_assembly_11"/>
		<map name= 	"full_assembly_11">
		<area shape="rect" coords="0,0,300,300" alt="fa11" href= "/portfolio/public/images/full_assembly_11.png" target = "_blank">
		</map>
		<img src="/portfolio/public/images/full_assembly_render.png" style="background-color:white;" width="200" heigth="300" alt="fa10" usemap="#full_assembly_render"/>
		<map name= 	"full_assembly_render">
		<area shape="rect" coords="0,0,300,300" alt="fa10" href= "/portfolio/public/images/full_assembly_render.png" target = "_blank">
		</map>

		<img src="/portfolio/public/images/torsoP_2.jpg" style="background-color:white;"  width ="200" alt="torsoP_2" usemap="#torsoP_2"/>
		<map name= 	"torsoP_2">
		<area shape="rect" coords="0,0,300,300" alt="torsoP_2" href= "/portfolio/public/images/torsoP_2.jpg" target = "_blank">
		</map>

		<img src="/portfolio/public/images/torsoP_3.jpg" style="background-color:white;"  width ="200" alt="torsoP_3" usemap="#torsoP_3"/>
		<map name= 	"torsoP_3">
		<area shape="rect" coords="0,0,300,300" alt="torsoP_3" href= "/portfolio/public/images/torsoP_3.jpg" target = "_blank">
		</map>


		<img src="/portfolio/public/images/torsoP_1.jpg" style="background-color:white;" width ="200" alt="torsoP_1" usemap="#torsoP_1"/>
		<map name= 	"torsoP_1">
		<area shape="rect" coords="0,0,300,300" alt="torsoP_1" href= "/portfolio/public/images/torsoP_1.jpg" target = "_blank">
		</map>
		<br> <br>


		<b> Yes! to  Raspberry PI Zero W  .... Heck Nah! to Arduino UNO </b> <br>
		In addition to the pretty pictures above, the software has been slowly developing.
		Settling on a Raspberry Pi Zero W, I will still control the motors over serial via a microcontroller. However, after some testing, I soon realized that the UNO needs to go. Why?: <br>
		<ul>
			<li>
		Not nearly enough timers/PWM's (Only 6 PWM's with one timer occupied by millis()
		And being 8 bit (two PWMs can be 16 bit) means I can't get exact frequencies unless I use a special mode that customizes the TOP of the counter. This just means low resolution of the Output Compare (PWM).</li>
		</ul>
		So long story short, I need more PWM's, GPIO's and 16 or 32 bit timers. <br><br>

		<b>Libraries, Screens, and cameras... </b><br>
		As for the rest of the system here is what I've been able to do:
		<ol>
		<li>
		Created a test bed on a Raspberry Pi 3 using a virtual environment running python 2.7 (for older libraries) and OpenCV 3.0. 
		</li> <br> 
		<li> Transferred over some motor control libraries to C and tested them on the UNO 
		</li> <br> 
		<li> Developed a multithreaded system running face recognition using the Pi Camera with Python handles from picamera.array() to get raw data!
		</li> <br>
		<li> Received my tft touchscreen from Itead.cc which I am currrently writing a Python wrapper using boost-python</li>
		</ol>

		until next time...





</li>
</ul>
</p>
     </div>
 </div>


 <div class="accordion">
 <h3>April 14th 2017</h3>  
     <div>
       <p>
<ul>
<li>
This week was so satisfying. I was able to print the first couple prototypes after CADing the upper arm, tweaking the mechanics just right to get them to fit, waiting on parts to ship from HongKong/everywhere and reCADing to fix some small errors. And as of April 10th I have it.. pretty much running. Even better, I was able to test out most of the design flaws! 
As I wrapped up the upper Arm, I finally got the CAD done on the lower arm. This really took alot of doing because the mechanics were so hard to fit. I ended up widening the forearm/lower arm. I still have some minor adjustments to do to make sure all the tolerances are right for the print, but the bulk of the work on the arm is DONE!
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
</ul> </p>
</div>
</div>

 <div class="accordion">
 <h3>April 10th 2017</h3>  
     <div>
       <p>
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

</p>
</div>
</div>

 <div class="accordion">
 <h3>April 4th 2017</h3>  
     <div>
       <p>

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
</p>
</div>
</div>

Background image credit: skyandtelescope.com


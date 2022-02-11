---
layout: page
title: Kod*Lab Mjbots SDK
description: Developing an opensource SDK for creating dynamic legged machines using the Mjbots motor controllers
img: assets/img/tvh_proto.jpg
importance: 3
category: Kod*Lab
---

The goal of this project was to find an open source alternative to commercially
available high performance BLDC motor driver + control frameworks. After discovering
<a href="https://mjbots.com/">Mjbots</a> which satisfied the hardware needs, the goal
shifted to creating an SDK which allowed for communication at 1kHz with the motors, logging,
and the ability to communicate with the robot from a laptop. This project 
served as an opportunity for me to explore modern C++, concurrency, and realtime computing.
The resulting SDK can be found here: 
<a href="https://github.com/KodlabPenn/kodlab_mjbots_sdk">https://github.com/KodlabPenn/kodlab_mjbots_sdk</a>

The kodlab_mjbots_sdk has a few key key features added to the 
pi3_hat library developed by mjbots: <a href="https://github.com/mjbots/pi3hat">https://github.com/mjbots/pi3hat</a>

1. Cross compiling support from ubuntu 20.04 to Raspberry pi
2. Integration with NYU realtime_tools library:<a href="https://github.com/machines-in-motion/real_time_tools">https://github.com/machines-in-motion/real_time_tools</a>
for better realtime performance
3. Integration with LCM (<a href="https://lcm-proj.github.io/">https://lcm-proj.github.io/</a>) for remote logging and remote input to the robot
4.  The `MjbotsControlLoop` object which handles the structure of the control loop for
the easy creation of new controllers
5. The `MjbotsRobotInterface` which provides a convenient interface for communicating with any number
of moteus motor controllers 


In order to test the SDK we used it to develop a simple demo hopper. The
source code for the demo hopper can be found here:
 
 <a href="https://github.com/KodlabPenn/kodlab_mjbots_sdk/blob/master/examples/leg_example.cpp/">https://github.com/KodlabPenn/kodlab_mjbots_sdk/blob/master/examples/leg_example.cpp</a>
 <div class="row">
     <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/9TqnH6Hkhok" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>

Going forward I aim to add support for limb level control to the `MjbotsRobotInterface`
and allow for sending PD commands to the motors in addition to just torques.



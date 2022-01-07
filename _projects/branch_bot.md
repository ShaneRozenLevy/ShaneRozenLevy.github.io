---
layout: page
title: Branch Bot
description: a soft, caterpillar-inspired, branch crawling robot
img: assets/img/branch_bot.jpg
importance: 1
category: Soft Robotics
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/branch_bot.jpg title: "branch bot" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>

Branch Bot is a biomimetic soft robot designed to study caterpillar locomotion. 
It has three soft passive grippers and two springy body segments. It is actuated using offboard 
motor tendon systems which connect to the robot using Bowden cables. The motor tendon system are controlled
to act like muscles. The robot's soft body allows it to crawl along branches using the same 
gait it uses for straight dowels. At the time of publication, Branch Bot was one of the fastest branch/tree climbing
soft robots.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/Mc6VNxqdB7U" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>

<div class="caption">
    A video of the tethered version of branch bot crawling horizontally, vertically, and on branches.
</div>

Later as part of my MS Thesis I made Branch Bot untethered by moving the control, power, and actuation onboard.
As a part of this process I designed and manufactured a simple closed loop motor control unit which did position control
on two DC motors and received inputs over I2C.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/branch_botU.jpg title: "branch bot" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    The untethered version of Branch Bot
</div>


<div class="publications">
  <h2>Associated Publication</h2>
  {% bibliography -f papers -q @*[project=branch_bot]* %}
</div>

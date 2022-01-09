---
layout: page
title: Tail Energized Hopping with Jerboa
description: replicating previous controllers on Jerboa
img: assets/img/jerboa.JPG
importance: 1
category: Kod*Lab
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/jerboa.JPG title: "jerboa" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>

Jerboa is a tailed biped with springy legs and a high powered 2 degree of freedom tail.
This novel design allows us to ask questions about how a high powered tail
might compensate for low degree of freedom legs. By working with a robot that
can't function without its tail, we can learn about different ways to take 
advantage of core actuation in ways that can be applied to spined quadrupeds.


The goal of this work is to replicate the previous work done by Avik De on Jerboa.
To start I implemented a pitch unlocked tail energized gait on the boom.

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/yyfhOc1Eo54" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>    </div>
</div>

Next I worked on using the tail to stabilize roll. In the following video I drop
the robot and let the tail reorient the robot while also reaching a position
that sets the tail up to be used for hopping.

 <div class="row">
     <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/lJk1__zjv1I" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe> 
    </div>
</div>

---
layout: page
title: Agile Jumping with a 12 dof Quadruped
description: Using Drake & DIRCON to design agile behaviors for a quadruped
img: assets/img/quadruped.png
importance: 2
category: Kod*Lab
---

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% responsive_image path: assets/img/quadruped.png title: "12 dof quadruped" class: "img-fluid rounded z-depth-1" %}
    </div>
</div>

In this project we explored applying trajectory optimization to enabled a 12-dof quadruped to 
jump. By using trajectory optimization we would understand how different designs
and gait sequences would effect a robot's ability to do agile maneuvers.
This work was conducted with Diego Caporale. 

This project also served as an opportunity of Kod*Lab to evaluate trajectory optimization
as a tool since we traditionally avoid optimization based techniques.


To start with we used Drake and DIRCON to design a pipeline for creating new
jumping behaviors. We started simple with jumping straight up.
 <div class="row">
     <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/sQydj9rh58E" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>

Before moving to jumping a longer distance forward and also optimizing for minimum energy.

 <div class="row">
     <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/el5e5tmCsys" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>

Before finally exploring different mode sequences with a bounding jump
 <div class="row">
     <div class="col-sm mt-3 mt-md-0">
        <iframe width="560" height="315" src="https://www.youtube.com/embed/8wWl00YvjMw" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
</div>

While trajectory optimization has enabled very impressive results, the resulting 
nonlinear programs are very difficult to get working well, leading to the work being
part science, and part art.


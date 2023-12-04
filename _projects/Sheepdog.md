---
layout: page
title: MyRIO Sheepdog Project
description: Coded using LabVIEW, the robot does line-following and herding using a myRIO microcontroller and PI controllers.
img: assets/img/sheepdog1.jpeg
importance: 1
category: courses
#related_publications: einstein1956investigations, einstein1950meaning
---
**Technical skills:** LabVIEW, PID controllers, Finite state machines

As part of the final project in _ME 375: Measurement and Control Systems II_, we had to build a sheepdog robot using a myRIO microcontroller. The specifications were: 

* The robot should follow the middle line around the track
* The robot should automatically change to its herding behavior after one lap around the track
* The robot should dynamically adjust the distance between itself and a moving obstacle, maintaining a distance of 9"
* The robot should use closed-loop feedback mechanisms to control the wheel velocities



<div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/sheepdog1.jpeg" title="Sheepdog Robot" class="img-fluid rounded z-depth-1" width = "300" %}
    </div>
</div>

<iframe width="420" height="315" src="https://youtube.com/embed/6c4U_io_qw4?si=DDrcKDmR8PRDzyCA" frameborder="0" allowfullscreen> </iframe>

The robot's operations were coded in LabVIEW using _Control & Simulation Loops_, with PI controllers to reduce the error between the desired and the measured wheel velocities. The operations within the line-following and herding behaviors were organized and coded using nested finite state machines. Our robot successfully exhibited the two behaviors; our final report can be found below.  


<iframe src="https://drive.google.com/file/d/15GJiOa5knQVytkxpyD7wyg9mFoFJafh9/preview" width="640" height="480" allow="autoplay"></iframe>
---
layout: page
title: Fluid Mechanics Open Lab Project
description: Investigating how the lift and drag coefficients change with the wing's angle of attack at different flight phases for the PA-180 airplane
img: assets/img/fluids1.png
redirect: 
importance: 3
category: courses
---
**Technical skills:** CAD (Solidworks), Experiment Design, CFD, MATLAB

As part of the open lab project in _ME 30801: Fluid Mechanics Laboratory_, we designed an experiment to investigate the effects of varying angles of attack (AoA) on the lift and drag coefficients at three flight phases. Our overarching motivation was to improve fuel efficiency and passenger experience through the aircraft performance. 

The flight phases we investigated are take-off, cruise, and landing. Dimensional analysis was used to scale down the actual wing to the model wing, with testing being conducted in a wind tunnel. Three models, corresponding to each flight phase, was designed and 3D printed, with each having a different AoA. Each phase also has a different wind speed. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fluidstakeoff.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fluidscruise.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fluidslanding.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    CAD designs of model wings
</div>

A stand was also created using dowel rods and 3D printed elbow attachments to secure the model wings to the wind tunnel's mount. The full testing assembly can be seen below:
<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/fluids1.png" title="example image" class="img-fluid rounded z-depth-1" width = "400"%}
    </div>
</div>
<div class="caption">
    Testing assembly
</div>

Experimental data was collected by adjusting the flight phase specific AoA by +/- 5 degrees. The readings were taken using a dynamometer and converted to voltage readings using a Linear Variable Differential Transformer (LVDT). Data processing and analysis were done using MATLAB. The correlation between experimental data and empirical data of the NACA 652-415 airfoil vary based on the AoA and the coefficient. We however did observe an increase in lift coefficients as the AoA increased, until a certain point, known as stalling. Some of our calculated drag coefficients were negative, and we reasoned that this could be due to systematic errors in the offsets. 

Our PowerPoint presentation and report can be found below:

<iframe src="https://docs.google.com/presentation/d/e/2PACX-1vTSQawDuVBWmSlVTBKzEU0MYhyGy6wlIYSmaxdtovk0FBqanzyiGJtMdLmK1H5zYYsNtFJiSvImkfae/embed?start=false&loop=false&delayms=3000" frameborder="0" width="640" height="375" allowfullscreen="true" mozallowfullscreen="true" webkitallowfullscreen="true"></iframe>

<iframe src="https://drive.google.com/file/d/1uNMVpNXNl4w5CH2eGIjP1CpFsPwEkF9f/preview" width="640" height="480" allow="autoplay"></iframe>

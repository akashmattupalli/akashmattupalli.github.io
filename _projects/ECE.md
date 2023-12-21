---
layout: page
title: Basic Audio Equalizer Project
description: Building an audio equalizer using low-pass, band-pass and high-pass filters
img: assets/img/ececircuit.jpg
importance: 4
category: courses
---
**Technical skills:** Circuit Design, MATLAB, LTSpice

As part of the final project in _ECE 20007: Electrical Engineering Fundamentals Lab_, we had to build a basic audio equalizer circuit using op-amps and low-pass, band-pass and high-pass filters. The specifications were: 

* Three filters have to be used: bass with cutoff at 320Hz, mid with range of 0.32kHz to 3200kHz, and treble with cutoff at 3.2kHz
* Amplifier output power has to be more than 400mW from 200Hz to 10khz
* Max ripple of 15 * mV_rms from 200Hz to 10kHz
* Volume control must be enabled

The tolerance margin of all the specifications were +/- 10%. To ensure that the combination of resistors, capacitors, and inductors fall within the tolerance margin, I coded a MATLAB program to help choose the components to build the circuit. The circuit was simulated and designed using LTSpice. 

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ece1.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ece2.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ece3.png" title="example image" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    LTSpice diagrams of the three filters, Low-Pass, Band-Pass and High-Pass from left to right
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/ececircuit.jpg" title="example image" class="img-fluid rounded z-depth-1" width = "400"%}
    </div>
</div>
<div class="caption">
    Basic audio equalizer circuit
</div>
The performance of the audio equalizer and its filters were tested using frequency response analysis using oscilloscopes. The results and procedure can be found in the report below: 

<iframe src="https://drive.google.com/file/d/1cTskAPL3wwVmm7B5TbqlOMrozPJRdkUu/preview" width="640" height="480" allow="autoplay"></iframe>

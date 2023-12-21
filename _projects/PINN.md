---
layout: page
title: Physics-Informed Neural Networks in non-Newtonian Thermal Greases
description: Simulating rheological tests to find out visco-elastic behaviors of DOWSIL TC-5622 and DOWSIL TC-5550 thermal greases
img: assets/img/PINN1.png
importance: 1
category: labs
---
**Technical skills:** Python (NumPy, DeepXDE, Pandas), Linear Algebra, Deep Learning, Linux

I worked as an undergraduate researcher for the _Transport: Modeling, Numerics & Theory Lab_ under Dr. Ivan Christov on his research in CFD and using machine learning to simulate rheological tests of thermal greases. My work in Fall 2023 has largely been understanding how to leverage DeepXDE neural networks and deep learning to effectively simulate accurate results with experimental data as training data. 

The first month of research was focused on collaborating with the graduate researchers to get up to speed on the relevant knowledge required on fluid mechanics and DeepXDE. 

The next couple of months were focused on simulating data with a single shear rate, and then expanding the training set to include multiple shear rates. After running the code through Google Colab, we transitioned to running the code in computer clusters at Purdue using Linux and the Anaconda module. Checkpoints were added in the code to save the models at every 100,000 iterations as they were being trained. 

<div>
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.html path="assets/img/PINN1.png" class="img-fluid rounded z-depth-1" width = "800" %}
    </div>
</div>
<div class="caption">
    Layout of the Physics-Informed Neural Network in DeepXDE
</div>

Most of the work went into fine-tuning the hyperparameters of the neural network to ensure the accuracy of the simulated results. Some of the factors included:

* Neural network architecture (number of hidden layers and number of neurons per layer)
* Number of data points taken for training
* Weights of the loss terms in the loss function
* Initial guesses of the neural network
* Number of iterations to train the model
* Constraining the data using initial conditions 
* training data points spaced out using np.linspace or np.logspace

An example of a Google Colab code can be found below:
<script src="https://gist.github.com/akashmattupalli/fc9899890edeb4c811881421de3578d3.js"></script>

I will be continuing my research with Dr. Ivan Christov next semester. My work will be focusing on fine-tuning the code for multiple shear rates further, before using Bayesian Inference model selection to perform uncertainty distribution analysis on the simulated results.
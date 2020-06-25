# PyCBC Inference Online Workshop 2020

In this workshop, we will provide tutorials on how to use PyCBC Inference to do parameter estimation with gravitational waves. Tutorials will involve going through jupyter notebooks that highlight how the various methods and functions in PyCBC Inference work, and how to use the exectuables to do gravitational-wave parameter estimation. We will also review basics of Bayesian inference and stochastic sampling, and their application to gravitational waves.

## Meeting location

We will hold the meeting via Zoom. We will email participants the connection information.

## Prerequisites

To run the tutorials, we will be using [SciServer](https://apps.sciserver.org). If you don't already have one, please create a SciServer account (it's free) before the meeting. 

### How to setup SciServer
*Note: we will go through the following instructions on Thursday morning, before going through the first tutorial. Feel free to do this ahead of time if you like, however.*
Go to https://apps.sciserver.org/compute/.
  1. Click "Create container". Give it a name. In the "Compute Image" drop-down menu make sure "SciServer Essentials" is selected. Then click "Create."
  1. Click on the container you just created; this will open a new tab in your browser that is a Jupyter notebook interface.
  1. All of the tutorials we will use are in the [PyCBC-Tutorials](https://github.com/gwastro/PyCBC-Tutorials) repository. Clone the PyCBC-Tutorials repository into your SciServer container: Click "New" -> "Terminal". This will open another tab that with a bash terminal in it. Change directory into "workspace" by typing `cd workspace`. Now type:
     ```
     git clone https://github.com/gwastro/PyCBC-Tutorials.git
     ```
     This will download a copy of this repository to your directory on SciServer.
  1. We will be using the `Workshop2020` tag of `PyCBC-Tutorials`. To ensure that you are using that tag, after the clone, change directory into "PyCBC-Tutorials" by typing `cd PyCBC-Tutorials`. Now type:
    ```
    git checkout tags/Workshop2020 -b Workshop2020
    ```
    This will checkout a local branch of the Workshop2020 release.
  1. Go back to your tab with the Jupyter notebook. Click on the "PyCBC-Tutorials" directory. From there you can navigate to the tutorial you want to view (using the itinerary below as a guide). When you click on a tutorial (files that end in `.ipynb`), a new tab will open with the tutorial open in it. All of the code needed is installed at the beginning of the tutorials.


## Itinerary (subject to change)

All times are CEST.

### Thursday 25 June
 * 11:00 - 12:00: Lecture
    * Introduction to Bayesian Inference and PyCBC Inference [keynote version](intro_to_bayesian_inference.key), [pdf version](intro_to_bayesian_inference.pdf)
 * 12:00 - 12:15: Setting up Sciserver
 * 12:15 - 14:30: break
 * 14:30 - 17:30: Tutorials
   * Learn about models and do parameter estimation in a notebook  (Inference #1)
   * PyCBC Inference code road map (Inference #2)
   * Using PyCBC Inference on an analytic test (Inference #3)

### Friday 26 June
 * 11:00 - 12:00: Tutorial
   * How to estimate the parameters of a binary black hole merger (Inference #4)
 * 12:00 - 13:00: break
 * 13:00 - 15:30
   * How to load, plot, and manipulate results (Inference #5)
   * Advanced configuration settings (Inference #6)
   * How to add custom waveforms to PyCBC (Inference #7)
 * 16:00 - 17:30: How to use PyCBC Inference in Condor workflow *Note: this session will focus on how to use the workflow on the Atlas cluster for members of the AEI Hannover, but will be instructive for anyone that has access to a condor-enabled cluster.*
   * Analyzing multiple events at once
   * Doing percentile-percentile tests and/or injection studies

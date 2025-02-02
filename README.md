# IKTBT-Release

This simulation is based on Unity 3D game engine software. It simulates a multi-robot search and rescue (or foraging) problem with different robots having different knowledge bases. For example, some robots know only to pick up red/blue/green/yellow targets, while some robots know all targets or no targets. All robots have basic collision avoidance and random walk routines in their knowledge base.
The simulator has key options for various modalities: 'No Interaction', 'Query-Response-Action', 'Query-Response-Update', 'Eavesdrop-Update', and 'Eavesdrop-Buffer-Update'

## Paper Citation
A paper describing the framework is available in ArXiv: https://arxiv.org/abs/2312.11802 

If you use/refer to our work, please consider citing the below paper.
Oruganti, S., Parasuraman, R., and Pidaparti, R., “IKT-BT: Indirect Knowledge Transfer Behavior Tree Framework for Multi-Robot Systems Through Communication Eavesdropping”, arXiv preprint arXiv:2312.11802. 2023

## Video Explanation  
Click below for a video presentation on IKT-BT works with a demonstration of BT transfers for various modalities.

[![Click for video](https://img.youtube.com/vi/xOJ8HIMnols/0.jpg)](https://youtu.be/xOJ8HIMnols)


## Installation
#### Note: This simulation software works only on Windows 10 and Windows 11 environments.  

Download the latest release [here (v4.2)]().  
After downloading the .zip file extract all the contents to a directory.  
Open the file BTTransferSimulator.exe  
You may have to click "More Info" and "Install Anyway" if your firewall blocks/scans the application.
**Note: If you are using an antivirus or antimalware software, you may have to add BTTransferSimulator.exe and LearnBTV1.exe files to the exclusion list.**  

Once you run the application - the simulator settings Frontend will pop up. Choose your settings as described below and click the "Run Simulations" button. 
**It will take some time to initialize and run the Unity-based simulations** (up to a minute in some cases at least in the first trial) and eventually it will create a new window with the simulation visualization. Please wait for this process.


## Simulator settings panel
![FrontEnd](https://github.com/sanjayovs/IKTBT-Release/blob/master/forReadme/FrontEnd.png)

<ins> Target Type:</ins> There are four target types in the simulator that are colored red, green, yellow and blue and have four corresponding zones at each corner  
<ins>Target Counts:</ins> The number of targets of each type to be initialized in the simulations.  
<ins>Obstacles:</ins> Check to add static obstacles  
<ins>Scenario:</ins> There are currently two scenarios available for the current study 
&nbsp; 
* No Interactions (NI)
* Query-Response-Actions (QRA)
* Query-Response-Update (QRU)
* Eavesdrop-Update (EU)
* Eavesdrop-Buffer-Update (EBU)  

<ins>Robot Types:</ins> There are 3 types of robots, 
&nbsp;  
1. I -Ignorant - Robots that have no initial knowledge about any of the targets
2. M - Multi-target - Robots that have knowledge about all the targets
3. R/G/Y/B - Single-target - Robots that have knowledge about red, green, yellow, and blue colors.

<ins>Communication Range:</ins> The range within which it can communicate with its neighbors. This is measured in times of the size of the robot.  
<ins>Total Trials:</ins> The number of trials to conduct for data collection  
<ins>Start Count:</ins> Starting trial number count for running simulations. This is to let the user continue simulations from the point they are stopped.  
<ins>Continuous:</ins> If unchecked, simulations stop after each trial and wait for the user to press the exit button on the simulator. If checked a trial instance is closed and a new trial instance is opened automatically.  
<ins>Parallel Instance Interval:</ins> This simulator supports parallel simulation instances. If set to a value more than 1 and if the trials are greater than 1 multiple simultaneous instances are initiated. For e.g., if the trials are 10 and the max parallel instance intervals are 3, only 3 instances are open at a time.  
**Note: Multiple parallel instances might slow down the simulations, hence a PC with good processing speed and a GPU is recommended**  

<ins>Duration:</ins> The maximum number of iterations before stopping. Each iteration has a fixed time of 0.01s.  
<ins>Targets:</ins> Stop after a certain overall percentage of targets are collected.  
<ins>No Stop:</ins> Simulations do not have stopping criterion.  
<ins>Record Data:</ins> Enable this to record data  
<ins>Auto Name:</ins> Auto Names the files and folders (Recommended)  
<ins>Save Path:</ins> Choose save directory for the recorded data.  
<ins>Config. File:</ins> Parameter summary  
<ins>Simulation Control:</ins> Run Simulations -> Click to run simulations after setting the parameters.  
<ins>Pause/ UnPause:</ins> Pause or unpause all instances of simulations  
<ins>Stop Simulations:</ins> Stop all the instances/ terminates all simulation instances.  
**Note: Do not press stop simulations while the instances are initializing**







## Simulation Instance
![SimulationInstance](https://github.com/herolab-uga/KTBT-Release/blob/master/forWiki/Simuloation.png)

The simulation parameters segment in an instant shows the parameters transferred from the settings form.

<ins>Camera View:</ins> Currently there are two views available.  
<ins># Robots that can handle:</ins> Counts of robots that have knowledge about each target type.  
<ins># Known Conditions:</ins> Number of robots that are ignorant (None), knowledge about 1, 2 3, and all targets respectively.  
<ins># Robot States:</ins> Number of robots in different states at a given point of time/ iteration.  


## Core contributors

* **Dr. Sanjay Sarma Oruganti Venkata** -- College of Engineering, University of Georgia (https://github.com/sanjayovs). Currently a postdoctoral researcher at Rensselaer Polytechnic Institute (RPI).

* **Prof. Ramviyas Parasuraman** -- HeRoLab, School of Computing, University of Georgia (https://hero.uga.edu)

* **Prof. Ramana Pidaparti** -- DICE Lab, College of Engineering, University of Georgia (https://dice.engr.uga.edu/)


## Heterogeneous Robotics (HeRoLab)

**Heterogeneous Robotics Lab (HeRoLab), School of Computing, University of Georgia.** 

For further information, contact Dr. Ramviyas Parasuraman ramviyas@uga.edu

https://hero.uga.edu/

<p align="center">
<img src="https://herolab.org/wp-content/uploads/2021/04/herolab_newlogo_whitebg.png" width="300">
</p>

# Deep Robot Learning from Demonstration (D-RLfD): A Dataset For Autonomous Robotic Suturing

<!-- TABLE OF CONTENTS -->
## Table of Contents

* [About the Project](#about-the-project)
* [Dataset Structure](#Dataset-Structure)
* [Models](#Models)
## About The Project

Suturing is a frequently used operation in most of the surgeries and developing a robotic system for autonomous robotic suturing can be of significant assistant to surgery team in order to reduce the physical fatigue and cognitive load. Since tissues are deformable objects needle insertion and tissue manipulation is a complex control task. The second complexity of the control task belongs to the high dimensional sensory data (Visual sensor) which makes the problem very hard for conventional control theory/Learning from Demonstration algorithms. We have collected a dataset for piercing needle into an artificial tissue with da Vinci Research Kit (DVRK) to develop deep LfD models for robot control.


## Dataset Structure

The dataset includes 60 folders including the corresponding data for 60 successful needle insertion trials executed by an expert. The operation is recorded by three pairs of stereo cameras (six cameras in total) and DVRK arms joint space and end-effector data are stored. The calibration parameters which include the relative pose of two cameras in each pair and pose of each camera relative to robots base frames are included in the dataset as well. The overla structure of robot data can be stated as follow:

<p align="center">
  <img width="700" src="images/cell(4).png">
</p>

a: joint space kinematic data of Arm 1 (1×6)

b: joint space kinematic data of Arm 2 (1×6)

c: pose of Arm 1 w.r.t its base frame (4×4)

d: pose of Arm 2 w.r.t its base frame (4×4)

e: pose of Arm 1 w.r.t its base frame at t+1 (4×4)

f: pose ofArm 2 w.r.t its base frame at t+1 (4×4)

g: 2D tracking target point on the image captured by 6 cameras(6×2)

h: computed 3D position of the target point w.r.t Camera 3(1×3)


## Models

Use this space to show useful examples of how a project can be used. Additional screenshots, code examples and demos would be great! You can also provide links to more resources. 

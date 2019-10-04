# ball_chaser
A ROS simulation of a robot equipped with a LiDAR and camera to 'chase' a white ball when in front of it.
This repository contains the code and the support files required for the simulation. 
Before running this simulation , the following is to be done for setting up the catkin workspace and catkin packages.
Ubuntu version : 16.04, ROS version:Kinetic
Steps:
1)Create a catkin_ws/src directory in your preferred location
$ mkdir -p /(path)/catkin_ws/src
2) Initialize a catkin workspace 
$ cd /(path)/catkin_ws/src
$ catkin_init_workspace
3)catkin_make is used to build code in catkin.

$ cd /home/workspace/catkin_ws
$ catkin_make
 A source and a devel repository will be created alongside src.

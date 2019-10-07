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

$ cd /(path)/catkin_ws
$ catkin_make
 A source and a devel repository will be created alongside src.

4)Create the my_robot package using the following commands:

$ cd /(path)/catkin_ws/src/
$ catkin_create_pkg my_robot

Clone the contents of the my_robot package into this package.


5) Create the ball_chaser package using the following:

$ cd /(path)/catkin_ws/src/
$ catkin_create_pkg ball_chaser roscpp std_msgs message_generation

Clone the contents of the ball_chaser package into this package.

6) Launch the robot:

$ cd /(path)/catkin_ws/
$ source devel/setup.bash
$ roslaunch my_robot world.launch

7)Run drive_bot and process_image

$ cd /(path)/catkin_ws/
$ source devel/setup.bash
$ roslaunch ball_chaser ball_chaser.launch


8)Visualize the results:

$ cd /(path)/catkin_ws/
$ source devel/setup.bash
$ rosrun rqt_image_view rqt_image_view  

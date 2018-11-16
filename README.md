# fasten-ur5
Simulation environment for ur5

# Description
This repository intends to provide a simulation environment (Gazebo+ROS+Rviz) for the development of pick and place functions with th UR5.

# Installation
Create a catkin workspace:

	$ source /opt/ros/kinetic/setup.bash
	$ mkdir -p ~/catkin_ws/src
	$ cd ~/catkin_ws/
	$ catkin_make
	$ source devel/setup.bash
   
Clone the git repository:

	$ git clone https://github.com/Ubira/fasten-ur5.git
		
Build the catkin workspace:

	$ cd ~/catkin_ws/
	$ catkin_make
	$ source devel/setup.bash
		
# Usage:
For simulation with Gazebo run the command:

	$ roslaunch ur5_gazebo ur5_setup.launch
		
The following world should appear in your Gazebo's GUI (make sure to start the simulation):

![alt text](https://github.com/Ubira/fasten-ur5/blob/master/images/Image1.png)
  

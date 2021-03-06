# fasten-ur5
Simulation environment for ur5

# Description
This repository intends to provide a simulation environment (Gazebo+ROS+Rviz) for the development of pick and place functions with the UR5.

It is based in the following packages:

https://github.com/utecrobotics/ur5

https://github.com/JenniferBuehler/common-sensors

https://github.com/utecrobotics/robotiq

https://github.com/philwall3/UR5-with-Robotiq-Gripper-and-Kinect

https://github.com/lihuang3/ur5_ROS-Gazebo

# Installation
Create a catkin workspace:

	$ source /opt/ros/kinetic/setup.bash
	$ mkdir -p ~/catkin_ws/src
	$ cd ~/catkin_ws/
	$ catkin_make
	$ source devel/setup.bash
   
Clone the git repository:

	$ cd ~/catkin_ws/src/
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
  
It's possible to run python scripts like "testmotion.py" with the command:

	$ rosrun ur5_gazebo testmotion.py

In case of writing a new script make sure to make it executable with (in the file folder):

	$ chmod +x YOUR_PYTHON_SCRIPT.py


# Robotic arm - Pick & Place project

As a part of Udacity Robotics Nano-Degree program, I had calculated the joint angles of a Kuka KR210 to solve the inverse kinematics problem. Simulation has been implemented in the ROS environmet with Gazebo and Rviz.

### Steps
* Set up your [ROS Workspace](http://wiki.ros.org/kinetic/Installation/Ubuntu).
* Download or clone the project repository into the src directory of your ROS Workspace from [here](https://github.com/udacity/RoboND-Kinematics-Project/blob/master/writeup_template.md)
* Experiment with the forward_kinematics environment and get familiar with the robot.
* Launch in demo mode.
* Perform Kinematic Analysis for the robot following the project rubric.
* Fill in the IK_server.py with your Inverse Kinematics code.

DH parameters had been derived from the urdf file and using them the homogenous transform between the base link and the end gripper had been found. From this the inverse kinematics equations are solved using trigonometric functions. Once all joint angles are found, the simulation was tested on the ROS environment with the help of IK_server.py.

After filling the IK_server.py with the code in the repository, you can launch the project via:

```
$ cd ~/catkin_ws/src/RoboND-Kinematics-Project/kuka_arm/scripts
$ ./safe_spawner.sh  
```

On a seperate terminal run the IK_server.py and click next on Rviz

```
$ cd ~/catkin_ws/src/RoboND-Kinematics-Project/kuka_arm/scripts
$ rosrun kuka_arm IK_server.py
```

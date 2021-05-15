# RoboticsND_MapMyWorld

This is repository for the fourth project of Udacity Robotics Software Engineer Nanodegree.

It includes two ROS packages:
* my_robot package - holds my robot and my world;
* teleop_twist_keyboard - [Teleop ROS package](https://github.com/ros-teleop/teleop_twist_keyboard) to control robot with keyboard

Additonally, we will be using an [RTAB-MAP package](http://wiki.ros.org/rtabmap_ros) to map the robot environment.

## How to try them out?

#### Create a catkin_ws
```sh
$ cd /home/
$ mkdir -p /home/catkin_ws/src/
$ cd catkin_ws/src/
$ catkin_init_workspace
$ cd ..
```

#### Clone the packages in catkin_ws/src/
```sh
$ cd /home/catkin_ws/src/
$ git clone https://github.com/NataliyaMish/RoboticsND_MapMyWorld.git master
```

#### Build the packages
```sh
$ cd /home/catkin_ws/ 
$ catkin_make
```

#### Source your environment
```sh
$ cd /home/catkin_ws/
$ source devel/setup.bash
```

#### Launch my_robot package
```sh
$ roslaunch my_robot world.launch
```

#### Run Teleop package to control the robot
```sh
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

#### Launch the mapping node to map the environment
```sh
$ roslaunch my_robot mapping.launch
```

#### Map the environment!
Use the keyboard commands and drive the robot around to generate a map of the environment.

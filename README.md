# RoboticsND_WhereAmI

This is repository for the second project of Udacity Robotics Software Engineer Nanodegree.

It includes three ROS packages:
* my_robot package - holds my robot and my world;
* pgm_map_creator package - [ROS package](https://github.com/udacity/pgm_map_creator) to create simulated world map in pgm format; 
* teleop_twist_keyboard - [Teleop ROS package](https://github.com/ros-teleop/teleop_twist_keyboard) to control robot with keyboard 

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
$ git clone https://github.com/NataliyaMish/RoboticsND_WhereAmI.git master
```

#### Build the packages
```sh
$ cd /home/catkin_ws/ 
$ catkin_make
```

#### After building the packages, source your environment
```sh
$ cd /home/catkin_ws/
$ source devel/setup.bash
```

#### Once the packages have been built, you can launch my_robot using
```sh
$ roslaunch my_robot world.launch
```

#### To launch AMCL package nodes to localize the robot
```sh
$ roslaunch my_robot amcl.launch
```

#### To run Teleop package to control the robot
```sh
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```

#### Localize the robot!
Use the keyboard commands and drive the robot around. 
In a short time you will see it localize itself - see example below.

**Step 1**
![Step 1](/screenshots/step1.png?raw=true)

**Step 2**
![Step 2](/screenshots/step2.png?raw=true)

**Step 3**
![Step 2](/screenshots/step3.png?raw=true)

**Step 4**
![Step 4](/screenshots/step4.png?raw=true)

**Step 5**
![Step 5](/screenshots/step5.png?raw=true)

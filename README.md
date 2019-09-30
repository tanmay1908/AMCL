# Using an Adaptive Monte Carlo Localization Algorithm in ROS and Gazebo

## Maintained by: Tanmay Agarwal
## Email: agarw139@umn.edu

-------

This repository allows you to simulate a robot in gazebo using an Adaptive Monte Carlo localization algorithm. The ROS amcl package is used for that purpose and the robot is simulated in a predesigned gazebo environment. 

The AMCL algorithm is a probablisitic approacch to robot localization in which it spawn multiple "nodes" in a known map and updates it's total set of nodes at regular intervals to only include those which are more "probable" to be at the true location of the robot. A representation from rviz is seen below:

![screenshots](/screenshots/SS_1.png)

This repo is the src directory of the catkin_ws. You will need to install ROS-Kinetic, Gazebo and the Rviz plugins to run the code succesfully. After that, navigate to the folder containing the repo (rename it src) and run the following commands on a terminal:
```
$ mkdir catkin_ws
$ mv src catkin_ws/src
$ cd catkin_ws/src
$ catkin_make
$ source devel/setup.bash
$ roslaunch main main.launch
```

This should now launch your simulation in RViz and keyboard teleop commands will open up in your terminal window

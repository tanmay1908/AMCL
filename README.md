#Using an Adaptive Monte Carlo Localization Algorithm in ROS and Gazebo

##Maintained by: Tanmay Agarwal
##Email: agarw139@umn.edu

-------

This repository allows you to simulate a robot in gazebo using an Adaptive Monte Carlo localization algorithm. The ROS amcl package is used for that purpose and the robot is simulated in a predesigned gazebo environment. 

The AMCL algorithm is a probablisitic approacch to robot localization in which it spawn multiple "nodes" in a known map and updates it's total set of nodes at regular intervals to only include those which are more "probable" to be at the true location of the robot. A representation from rviz is seen below:

![screenshots](/screenshots/SS_1.jpg)

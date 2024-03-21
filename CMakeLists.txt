cmake_minimum_required(VERSION 3.0.2)
project(ired_simulation)

find_package(catkin REQUIRED COMPONENTS
  gazebo_ros
  geometry_msgs
  nav_msgs
  roscpp
  rospy
  sensor_msgs
  std_msgs
  tf
  urdf
  xacro
)

################################################
## Declare ROS messages, services and actions ##
################################################

################################################
## Declare ROS dynamic reconfigure parameters ##
################################################


###################################
## catkin specific configuration ##
###################################

catkin_package(
 CATKIN_DEPENDS gazebo_ros geometry_msgs nav_msgs roscpp rospy sensor_msgs std_msgs tf urdf xacro
)

###########
## Build ##
###########

#############
## Install ##
#############

catkin_install_python(PROGRAMS
  scripts/teleop.py
  DESTINATION ${CATKIN_PACKAGE_BIN_DESTINATION}
)

#############
## Testing ##
#############


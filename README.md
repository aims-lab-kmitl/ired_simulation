# IRED SIMULATION
## Requirement Package
```
$ sudo apt install -y ros-noetic-slam-gmapping ros-noetic-map-server ros-noetic-amcl \
                      ros-noetic-move-base ros-noetic-navigation
```
## Command for IRED Robot
1. Open Gazebo
```
$ roslaunch ired_simulation gazebo.launch
```
2. Teleop
```
$ roslaunch ired_simulation teleop.launch
```
3. SLAM
```
$ roslaunch ired_simulation slam.launch
```
4. Save map
```
$ roslaunch ired_simulation savemap.launch
```
5. Navigation
```
$ roslaunch ired_simulation navigation.launch
```
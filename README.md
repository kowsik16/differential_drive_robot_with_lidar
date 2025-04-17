# differential_drive_robot_with_lidar (URDF + ROS 2 Jazzy Harmonic)
This repository contains the URDF and Xacro description of a differential drive robot equipped with LiDAR for autonomous navigation in ROS 2. The robot is designed for simulated navigation in Gazebo and visualization in RViz.(ROS 2 Jazzy Harmonic)

### Installation

### Clone the Repository:


cd ~/your_workspace_name/src 

git clone https://github.com/kowsik16/differential_drive_robot_with_lidar.git

### Install Dependencies:

sudo apt update && rosdep update

rosdep install --from-paths src --ignore-src -r -y


### Build the Package:

cd ~/your_workspace_name

colcon build --packages-select differential_drive_robot_with_lidar

source install/setup.bash


### Launch in RViz:

ros2 launch obslidar_description display.launch.py


### Launch in Gazebo:

ros2 launch obslidar_description gazebo.launch.py

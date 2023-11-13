# Autonomous-Mobile-Robot

 ## Additional required Packages:

 ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) To find imu_tools, visit: [imu_tools](https://github.com/CCNYRoboticsLab/imu_tools) <br />
 ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) To find rosserial and install it, visit: [rosserial](http://wiki.ros.org/rosserial_arduino/Tutorials/Arduino%20IDE%20Setup) <br />
 ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) To find robot_pose_ekf, visit: [robot_pose_ekf](http://wiki.ros.org/robot_pose_ekf) <br />
 ![#c5f015](https://placehold.co/15x15/c5f015/c5f015.png) To find rplidar_ros, visit: [rplidar](https://github.com/Slamtec/rplidar_ros) <br />
    
## Firmware:
 ![#f03c15](https://www.iconsdb.com/icons/download/color/f03c15/circle-16.png) See :arrow_right: [cytron_motor_driver](https://github.com/unipolarautomation/mobile_robot/tree/main/firmware/cytron_motor_driver) <br />

## Installation Process :toolbox:

 - create a workspace and Compile <br />

```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
```

![#f03c15](https://www.iconsdb.com/icons/download/color/f03c15/circle-16.png) Follow the procedure of ***rosserial*** installtion from here :arrow_right: [rosserial](http://wiki.ros.org/rosserial_arduino/Tutorials/Arduino%20IDE%20Setup) <br />

- go to `src` folder and clone: <br />

```
git clone https://github.com/unipolarautomation/mobile_robot.
git clone https://github.com/CCNYRoboticsLab/imu_tools.git
git clone https://github.com/ros-planning/robot_pose_ekf
git clone https://github.com/Slamtec/rplidar_ros
```

- go to `catkin_ws` folder and do: <br />
``` 
catkin_make
```
- run <br />
```
source devel/setup.bash
```
:trollface:

## Running the robot :rocket:
- Go to workspace `catkin_ws`
- Run 
```
source devel/setup.bash
```
- Run the launch file
```
roslaunch robot_bringup real_bringup.launch
```
- Run teleop_twist_keyboard in new terminal for running the robot using keyboard
```
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
:purple_circle: To install teleop_twist_keyboard, Run: <br />
```
sudo apt-get install ros-<ros distro>-teleop-twist-keyboard
```
- To run rviz:
```
rosrun rviz rviz
```




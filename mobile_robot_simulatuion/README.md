# mobile_robot_simulatuion

## Installation Process :toolbox:

 - create a workspace and Compile <br />

```
mkdir -p ~/catkin_ws/src
cd ~/catkin_ws/
catkin_make
```
- go to `src` folder and clone: <br />

```
git clone https://github.com/unipolarautomation/mobile_robot_simulatuion.git
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
roslaunch test_urdf_description gazebo.launch
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
- To run navigation launch file, run below command in new terminal:
```
roslaunch test_urdf_description move_base.launch
```
- To run amcl launch file, run below command in new terminal:
```
roslaunch test_urdf_description amcl.launch
```

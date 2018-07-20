
```
Create Catkin Workspace:
mkdir -p /home/workspace/catkin_ws/src
cd /home/workspace/catkin_ws/src
catkin_init_workspace
cd ..
catkin_make

apt-get update
apt-get upgrade -y

Clone Package:
cd /home/workspace/catkin_ws/src
git clone https://github.com/turtlebot/turtlebot_simulator

cd /home/workspace/catkin_ws
source devel/setup.bash
rosdep -i install turtlebot_gazebo

catkin_make
source devel/setup.bash

roslaunch turtlebot_gazebo turtlebot_world.launch

rostopic list
Or
rosrun rqt_graph rqt_graph


Install the package:
$ cd /home/workspace/catkin_ws/src/
$ git clone https://github.com/udacity/robot_pose_ekf
```

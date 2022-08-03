# Task_2

# Installing_robot_arm_package
###### First: open terminal to write command
###### Second: by yhe following command: we can ceate a new folder with the name catkin_ws, inside it create a folder named src:
> cd ~/catkin_ws/

> catkin_make

> cd ~/catkin_ws/src

###### Third: To download the backages insdie catkin_ws/src folder:

> git clone https://github.com/smart-methods/arduino_robot_arm.git 

###### Then: 
> cd ~/catkin_ws

> rosdep install --from-paths src --ignore-src -r -y

> sudo apt-get install ros-noetic-moveit

> sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui

> sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher

> sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

###### After that: Edit the file bachrc by:

> sudo nano ~/.bashrc

###### Then: Add the following source to the end of this file:
> source /home/"username"/catkin_ws/devel/setup.bash

-> for me (I have changed my name Zina instead of username )

-> source /home/"zeina"/catkin_ws/devel/setup.bash

###### Don`t forget to press ctrl+o to save changes, then write this command:
> source ~/.bashrc

###### Finally: we can launch RIVz by following command:
> roslaunch robot_arm_pkg check_motors.launch


# ROS Melodic Install

## Install Packages

```
$ sudo sh -c 'echo "deb http://packages.ros.org/ros/ubuntu $(lsb_release -sc) main" > /etc/apt/sources.list.d/ros-latest.list'
```

## Download Packages Keyserver

```
$ sudo apt-key adv --keyserver 'hkp://keyserver.ubuntu.com:80' --recv-key C1CF6E31E6BADE8868B172B4F42ED6FBAB17C654
```

## Updates Packages Index
```
$ sudo apt update
```

## Installation- ROS Melodic
```
$ sudo apt install ros-melodic-desktop-full

$ apt search ros-melodic
```

## Environment Setup
```
$ echo "source /opt/ros/melodic/setup.bash" >> ~/.bashrc

$ source ~/.bashrc
```

## Building Packages 
```
$ sudo apt install python-rosdep python-rosinstall python-rosinstall-generator python-wstool build-essential
```

## Initialize rosdep
```
$ sudo apt install python-rosdep

$ sudo rosdep init

$ rosdep update
```

## Catkin
```
$ mkdir -p ~/catkin_ws/src

$ cd ~/catkin_ws/

$ catkin_make
```

## ROS_Turtlesim_Test
```
$ roscore
```

### open a new terminal 2
```
$ rosrun turtlesim turtlesim_node
```

### open a new terminal 3
```
$ rosrun turtlesim turtle_teleop_key
```




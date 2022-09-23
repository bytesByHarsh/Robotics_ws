# ROS workspace

This repository includes sample codes to create your own robot using ROS.

All the bots related to my talk ["Build Custom Robot in ROS"](https://www.youtube.com/watch?v=cuNEOtLbB14) in [Pycon Sweden](https://www.pycon.se/) is also added.

## Contents

- [Prerequisites](#prerequisites)
- [Set Up](#set-up-workspace)
- [Atom Bot](#atom-robot)
- [Atom SDF](#atom-robot-sdf)
- [Beta Bot](#beta-robot)
- [Control Bots](#control-the-bot)
- [Autonomous Navigation](/docs/Navigation.md)

## Prerequisites

Replace <version> with noetic, melodic etc.
  
- ROS (`$ sudo apt-get install ros-<version>-desktop-full`)
- Xacro (`$ sudo apt-get install ros-<version>-xacro`)
- Gazebo (`$ sudo apt-get install ros-<version>-gazebo-ros`)

## Set up workspace


```bash
git clone https://github.com/harshmittal2210/Robotics_ws/
cd Robotics_ws
git submodule update --init --recursive
catkin_make
source devel/setup.sh
```

`Note: Do not add Robotics_ws in your catkin_ws/src`

I am just using the folder name `Robotics_ws` instead of `catkin_ws`

## Atom Robot

```bash
roslaunch atom world.launch
```
<p align="center">
<img src="./docs/img/atom.JPG" alt="Atom Bot" width="600"/>
  </p>

## Atom Robot (SDF)

```bash
roslaunch atom gazebo_world.launch
```
<p align="center">
<img src="./docs/img/atom1.JPG" alt="Atom Bot" width="600" />
  </p>
  
## Beta Robot

```bash
roslaunch beta_description gazebo.launch
```
  <p align="center">
    <img src="./docs/img/beta.JPG" alt="Atom Bot" width="400" />
    <img src="./docs/img/beta1.JPG" alt="Atom Bot" width="400"/>
    <img src="./docs/img/beta4.JPG" alt="Atom Bot" width="400" />
  </p>

## Control the bot

Use `teleop_twist_keyboard`

```bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=/atom/cmd_vel
```

## Autonomous Navigation

Refer to doc here: [Navigation](/docs/Navigation.md)
  
## Author

👤 Harsh Mittal

Twitter: [@harshmittal2210](https://twitter.com/harshmittal2210)
Github: [@harshmittal2210](https://github.com/harshmittal2210)
Website: [harshmittal.co.in](http://harshmittal.co.in)
  
## 🤝 Contributing

Contributions, issues and feature requests are welcome!

## Show your support

Give a ⭐️ if you think this project is awesome!

## 📝 License

Copyright © 2021 [Harsh Mittal](https://github.com/harshmittal2210).
This project is [Apache License](https://github.com/harshmittal2210/Robotics_ws/blob/main/LICENSE) licensed.

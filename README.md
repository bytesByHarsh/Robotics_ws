# ROS workspace

This repository includes sample codes to create your own robot using ROS.

All the bots related to my talk "Build Custom Robot in ROS" in Pycon Sweden is also added.

## Prerequisites

Replace <version> with noetic, melodic etc.
  
- ROS (`$ sudo apt-get install ros-<version>-desktop-full`)
- Xacro (`$ sudo apt-get install ros-<version>-xacro`)
- Gazebo (`$ sudo apt-get install ros-<version>-gazebo-ros`)

## Set up workspace

```bash
git clone <repo_link>
cd <repo_name>
catkin_make
source devel/setup.sh
```

## Atom Robot

```bash
roslaunch atom world.launch
```

## Atom Robot (SDF)

```bash
roslaunch atom gazebo_world.launch
```

## Beta Robot

```bash
roslaunch beta_description gazebo.launch
```

## Control the bot

Use `teleop_twist_keyboard`

```bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
  
## Author

👤 Harsh Mittal

Twitter: [@harshmittal2210](https://twitter.com/harshmittal2210)
Github: [@harshmittal2210](https://github.com/harshmittal2210)
Website: [harshmittal.tech](http://harshmittal.tech)
  
## 🤝 Contributing

Contributions, issues and feature requests are welcome!

## Show your support

Give a ⭐️ if you think this project is awesome!

## 📝 License

Copyright © 2021 [Harsh Mittal](https://github.com/harshmittal2210).
This project is [Apache License](https://github.com/harshmittal2210/Robotics_ws/blob/main/LICENSE) licensed.

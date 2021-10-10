# PyCon-Sweden-2021

ROS workspace

This repo includes smaple codes to create your own robot using ROS.

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


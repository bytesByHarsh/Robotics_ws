# Navigation

## Installation

```bash
sudo apt install ros-noetic-dwa-local-planner
sudo apt install ros-noetic-gmapping
```

# GMapping


## Implementation

Terminal 1:

```bash
roslaunch atom gmapping_demo.launch
```

Terminal 2:

```bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=/atom/cmd_vel
```

Move around the bot till you have scanned the complete room. Now in order to save the map use the following 
command

Terminal 3:
```
cd <location to save map>
rosrun map_server map_saver -f map
```
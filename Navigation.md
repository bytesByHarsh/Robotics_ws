# Navigation

## Installation

```bash
sudo apt install ros-noetic-dwa-local-planner
sudo apt install ros-noetic-gmapping
```

# GMapping


## Mapping

Terminal 1:

```bash
roslaunch atom gmapping_demo.launch
```

Terminal 2:

```bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=/atom/cmd_vel
```

![Gmapping Demo](/docs/img/gmapping.png)

Move around the bot till you have scanned the complete room. Now in order to save the map use the following 
command

Terminal 3:
```
cd <location to save map>
rosrun map_server map_saver -f map
```

![Scan](/docs/img/aws_scan.png)

# AMCL

Terminal 1:

```bash
roslaunch atom localization.launch
```

Terminal 2:

```bash
rosrun teleop_twist_keyboard teleop_twist_keyboard.py cmd_vel:=/atom/cmd_vel
```

Now you after moving bot a little you will be able to see that it is able to localize itself properly.

![Localization](/docs/img/localization.png)

# Navigation

Terminal 1:

```bash
roslaunch atom navigation.launch
```

Use RVIZ for 2D Navigation

![Give Navigation](/docs/img/navigation1.png)
![Robot goes to point](/docs/img/navigation2.png)
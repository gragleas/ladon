System: Ubuntu 22.04

Requirements:

  ROS2 >= Humble
  
  Python3 >= 3.8
  
  gz sim >= 7

1. Clone Repository

```
git clone https://github.com/gragleas/ladon.git --recursive
cd ladon
```

2. Build Wave Plugins and source

```
cd gz_ws
colcon build
source install/setup.bash
```

3. Make PX4 Target

Start QGroundControl in another window before this step.

```
cd ../PX4-Autopilot
make px4_sitl gz_boat PX4_GZ_WORLD=waves_wind
```

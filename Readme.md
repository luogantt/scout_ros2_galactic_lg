


# 或者你直接下载我调整好的
```
git clone https://github.com/luogantt/scout_ros2_galactic_lg
```

```
 cd scout_ros2_galactic_lg
 colcon build
```

#打开can 口

```
 sudo modprobe gs_usb
 ```

```
 sudo ip link set can0 up type can bitrate 500000
```

```
 sudo ip link set can0 up type can bitrate 500000
```

```
 sudo apt install can-utils
```

```
candump can0
```


Launch ROS nodes

Start the base node for the Scout robot

`ros2 launch scout_base scout_base.launch.py`
Start the keyboard tele-op node

`ros2 run teleop_twist_keyboard teleop_twist_keyboard`

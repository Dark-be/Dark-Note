# ROS2

## ROS2(Dashing)

* **Work with jetson nano.**

***

### Micro-XRCE-DDS-Agent(for microROS)

* Q : 某共享库缺失。
* A

```sh
ldconfig
```

### rplidar_ros2

> [rplidar_ros2]()

* 需修改 **.launch** 文件：**execute => node_execute**

### cartographer | cartographer_ros

> [cartographer_ros]()

* 编译**absl**需**Ninja**

* Q : **FindPackageShare cannot import** (来自鱼香**ROS**)
* A : 修改为

```python
  configuration_directory = LaunchConfiguration('configuration_directory',default= os.path.join(get_package_share_directory('fishbot_cartographer'), 'config') )
  from ament_index_python.packages import get_package_share_directory
```

## ROS2(Humble)

### Velodyne

> [velodyne](https://github.com/ros-drivers/velodyne/tree/humble-devel)

* 网线连接报错**activation faild**，修改**IPv4**地址

* 雷达默认**IP** 192.168.1.201
* 浏览器进入配置界面配置参数并保存
* **velodyne driver**中的**conf/*.yaml**需修改为雷达**IP**
* 启动**rviz**可视化，需修改**frameid**为**velodyne**

## MicroROS

* **Work with ESP32**

***


# ROS 日志记录
## ROS/ROS2
### 导航
ROS/ROS2社区[ros.index](https://index.ros.org/)
Project:
* >[ROS-Car-2022C](https://github.com/Dark-be/ROS-car-2022C)
### 注意事项
1. 卸载cmake会造成ros崩溃需重装
***
### ROS2
#### 安装编译Micro-XRCE-DDS-Agent(for microROS)
问题 某共享库缺失，解决方案：ldconfig
(esp32 microros)
#### 安装编译rplidar_ros2
.launch文件：**execute => node_execute**
#### 安装编译cartographer | cartographer_ros
1. 编译absl需**Ninja**

2. 问题 来自鱼香ROS **FindPackageShare cannot import**
* 改为**configuration_directory = LaunchConfiguration('configuration_directory',default= os.path.join(get_package_share_directory('fishbot_cartographer'), 'config') )**
* 改为**from ament_index_python.packages import get_package_share_directory**
***
### ROS
#### 关于多机通信
**export ROS_MASTER_URI:IP of master:11311**
**export ROS_HOSTNAME:IP of slave**
(**export ROS_IP**)
#### 关于cv_bridge
详见opencv_test包
可直接apt安装，使用需更改**cv_bridgeConfig**，指向本地opencv对应版本include_dir
#### robot EKF
#### Navgation
#### Robot Localization
####
***
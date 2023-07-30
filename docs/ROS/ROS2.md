# ROS2
## 安装编译Micro-XRCE-DDS-Agent(for microROS)
问题 某共享库缺失，解决方案：ldconfig
(esp32 microros)
## 安装编译rplidar_ros2
.launch文件：**execute => node_execute**
## 安装编译cartographer | cartographer_ros
1. 编译absl需**Ninja**

2. 问题 来自鱼香ROS **FindPackageShare cannot import**
* 改为**configuration_directory = LaunchConfiguration('configuration_directory',default= os.path.join(get_package_share_directory('fishbot_cartographer'), 'config') )**
* 改为**from ament_index_python.packages import get_package_share_directory**

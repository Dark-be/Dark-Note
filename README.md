# Dark-Note
Learning notes directory

## Document

[Dark-Note](https://Dark-be.github.io/Dark-Note)

***
[toc]
***
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
esp32 microros udp已连接成功
#### 安装编译rplidar_ros2
.launch文件：**execute => node_execute**
#### 安装编译cartographer | cartographer_ros
1. 编译absl需**Ninja**

2. 问题 来自鱼香ROS **FindPackageShare cannot import**
* 改为**configuration_directory = LaunchConfiguration('configuration_directory',default= os.path.join(get_package_share_directory('fishbot_cartographer'), 'config') )**
* 改为**from ament_index_python.packages import get_package_share_directory**
***
### ROS
#### 关于cv_bridge
详见opencv_test包
可直接apt安装，使用需更改cv_bridgeConfig，指向本地opencv对应版本include_dir
#### robot EKF
#### Navgation
#### Robot Localization
####
***
## K210
### 导航
示例代码[What is MaixPy3?](https://wiki.sipeed.com/soft/maixpy3/zh/index.html)
***
### 硬件加速
**img.conv3(kernel)**

kernel为卷积核，以下分别是原始图像，边缘检测，锐化，浮雕化卷积核:
* **origin = (0,0,0, 0,1,0, 0,0,0)**
* **edge = (-1,-1,-1,-1,8,-1,-1,-1,-1)**
* **sharp = (-1,-1,-1,-1,9,-1,-1,-1,-1)**
* **relievo = (2,0,0,0,-1,0,0,0,-1)**
***
## MCU
### 导航
***
### Tiva
#### MSP430/MSP432

#### TM4C129
Project:
* >[WHU-Car-Driver]()
#### TM4C123
***
### FreeRTOS
***
## Git
使用SSH密钥，更稳定，详见[Connecting to GitHub with SSH](https://docs.github.com/en/authentication/connecting-to-github-with-ssh)
***



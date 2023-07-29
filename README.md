# Dark-Note
my learning notes

## ROS/ROS2
卸载cmake会造成ros崩溃
### 安装编译Micro-XRCE-DDS-Agent
问题 连github失败，解决方案：从cmake文件里改url，使用gitee

问题 共享库缺失，解决方案：ldconfig
esp32 microros udp连接成功
### 安装编译rplidar_ros2
launch文件需修改execute->node_execute

安装编译cartographer | cartographer_ros
编译absl需Ninja

问题 来自鱼香肉丝 FindPackageShare cannot import 寻找包的路径函数需更新
改后configuration_directory = LaunchConfiguration('configuration_directory',default= os.path.join(get_package_share_directory('fishbot_cartographer'), 'config') )
改后from ament_index_python.packages import get_package_share_directory

## ROS2(Dashing)
***
#### Micro-XRCE-DDS-Agent(for microROS )
* Q : 某共享库缺失
* A : ldconfig
#### rplidar_ros2
* 需修改 **.launch** 文件：**execute => node_execute**
#### cartographer | cartographer_ros
* 编译**absl**需**Ninja**

* Q : **FindPackageShare cannot import** (来自鱼香**ROS**)
* A : 修改为
```python
  configuration_directory = LaunchConfiguration('configuration_directory',default= os.path.join(get_package_share_directory('fishbot_cartographer'), 'config') )
  from ament_index_python.packages import get_package_share_directory

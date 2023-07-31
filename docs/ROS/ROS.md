## ROS(Melodic)
* work with jetson nano
***
#### Work with MCU
* 与下位机串口通信，详见[serial_pkg]()
* 可重写**Ctrl-C**中断函数，实现ROS终止后执行结束指令
#### cv_bridge
* 可直接apt安装，使用需更改**cv_bridgeConfig**，指向本地**opencv**对应版本的**include_dir**
* 使用**opencv**图像处理以及图像信息转换发送，详见[opencv_test]()
#### robot EKF
#### navgation
#### robot localization
# ROS(Melodic)

* **work with jetson nano.**

***

## Work with MCU

* 与下位机串口通信，见[serial_pkg]()
* 可重写**Ctrl-C**中断函数，实现**ROS**系统终止前执行结束指令。

## Work with other device

* 同一网络下主从机话题通信。

```sh
export ROS_MASTER_URI=http://localhost:11311    #master
export ROS_HOSTNAME=localhost

export ROS_MASTER_URI=http://master:11311       #slave
export ROS_HOSTNAME=localhost
```

## rosdep(c)

* 自动安装**ROS**包依赖。

## packages

### cv_bridge

* 可直接apt安装，使用需更改**cv_bridgeConfig**，指向本地**opencv**对应版本的**include_dir**。
* 使用**opencv**图像处理以及图像信息转换发送。详见[opencv_test]()

### rplidar

> [rplidar_ros](#github)

### robot pose EKF

> [robot]()

### navgation

> [navgation]()

### robot localization

> [robot_localiztion]()

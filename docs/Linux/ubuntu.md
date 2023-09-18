# Ubuntu

## Ubuntu 18.04

***

## Tips

### Set static WLAN IP

* 查看网关等

```shell
ifconfig                #
route -n                #查看网关3
ipconfig/all            #Windows查看DNS
```

### Different Python interpreter version

* 存在不同**python**版本时 :

```sh
python -3.9 -m pip install pkg_name
```

### Configration

* 添加自己到**dialout**组，免去**tty**赋权

```sh
sudo usermod -aG dialout username
```

#### C++串口通信

* **CmakeLists**加入**ros-melodic-serial**(或者其他底层串口驱动)编译

## Ubuntu 22.04

### Install

* 使用**SD**卡和**balenaEtcher**烧录镜像
* 进入**BIOS**，设置**USB**启动即可开始安装

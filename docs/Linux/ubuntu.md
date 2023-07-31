## Ubuntu 18.04
Noticing some usage
***
#### Set static WLAN IP
* 查看网关等
```shell
ifconfig                #
route -n                #查看网关3
ipconfig/all            #Windows查看DNS

```
#### Different Python interpreter version
* 存在不同**python**版本时 :
```sh
python -3.9 -m pip install pkg_name
```
#### Configration
* 添加自己到**dialout**组，省去**tty**赋权
```sh
sudo usermod -aG dialout username
```


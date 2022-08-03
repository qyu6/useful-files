# Linux (Raspbian)
`shell`

更新密码
`'sudo passwd pi'`

调整vnc屏幕分辨率
`vncserver -geometry 1080*720`

打开vnc配置菜单
`sudo raspi-config`

给树莓派安装外设屏幕驱动
```
git clone https://github.com/waveshare/LCD-show.git
cd LCD-show/
sudo ./LCD35-show
```

显示当前温度
`vcgencmd measure_temp`

查找树莓派ip地址
`ping raspberrypi.local -4`

检查树莓派是否连接wifi成功
`ifconfig wlan0`

为树莓派添加新wifi
`
sudo nano /etc/wpa_supplicant/wpa_supplicant.conf
`

在文件底部添加新wifi信息
```
network={
ssid="The SSID of your network (eg. Network name)"
psk="Your Wifi Password"
}
ctrl x - y 保存后退出
```

显示当前文件路径
`pwd`

查看目录中的全部文件
`ls`

显示文件和目录中全部信息
`ls -l`

列出全部文件，包含隐藏文件
`ls -a` 

递归显示所有文件
`ls -R`

显示这个文件所有内容
`cat <file.name>`

获取网卡配置和系统的网络信息
`ifconfig`

---

安装python3.x</br>
`sudo apt install python3`</br>
`sudo apt remove python` #卸载python2.x


`sudo apt autoremove` #自动清理python2.x依赖


`sudo rm /usr/bin/python` #删掉原来python链接


`sudo ls -s /usr/bin/python3.7 /usr/bin/python` #创建一个新的链接


`python` #输入后自动进入python终端	

#linux文本编辑器 (nano/vim(是vi的增强版)/vi)


`nano` <file.name> #打开这个文件，并显示内容


`ctrl x` #退出 	

`vi <fine.name>` #通过vi编辑器打开文件

`:q` #退出编辑

`:q!` #强制退出

#树莓派默认的vi，没有颜色区分，使用上很不便捷
`sudo apt-get install vim #安装vim`

#更新raspbian系统
`sudo apt-get update`

#安装更新
`sudo apt-get upgrade
`

#树莓派安装mysql
`sudo apt-get install sqlite3`

`sudo apt-get install libsqlite3-dev` #安装sqlite3编译时需要的工具包

`sqlite3 -version` #检查sqlite3版本

`sqlite3` #输入进入sqlite环境



#树莓派安装spark
`wget https://www.apache.org/dyn/closer.lua/spark/spark-3.2.0/spark-3.2.0-bin-hadoop3.2.tgz` #下载安装包方法一

`curl -O https://www.apache.org/dyn/closer.lua/spark/spark-3.2.0/spark-3.2.0-bin-hadoop3.2.tgz` #下载安装包方法二

类似于wget/curl这种直接在linux系统中的下载方式，没有经过某些安装协议的要求。所以在linux环境汇中通过`tar -zxvf <file.name>.tgz` 的方式解压一直失败（后来发现这种方式下载的文件也不完整，只有几百k，但实际tgz文件有287MB）

解决办法，在windows系统中下载好，然后上传到linux服务器，再进行解压缩和安装操作
`tar zxvf spark-3.2.0-bin-hadoop3.2.tgz`

***


**第三步：一键加速VPS服务器**

五合一的TCP网络加速脚本，包括了BBR原版、BBR魔改版、暴力BBR魔改版、BBR plus（首选）、Lotsever(锐速)安装脚本。可用于KVMXen架构，不兼容OpenVZ（OVZ）。支持Centos 6+ / Debian 7+ / Ubuntu 14+，BBR魔改版不支持Debian 8。

***

```bash
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh"
chmod +x tcp.sh
./tcp.sh
```


***

> 如果提示 wget: command not found 的错误，这是你的系统精简的太干净了，wget都没有安装，所以需要安装wget。CentOS系统安装wget命令： yum install -y wget Debian/Ubuntu系统安装wget命令：apt-get install -y wget

安装完成后，脚本管理命令为：./tcp.sh

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/vultr/newbbr1.jpg)

操作方法：先安装内核，重启vps让内核生效，再启动对应的加速即可。数字1的BBR/BBR魔改内核对应数字4、5、6的BBR加速、BBR魔改加速和暴力BBR魔改版加速。数字2的BBRplus内核对应数字7的BBRplus加速。数字3的锐速加速内核对应数字8的锐速加速。（如果服务器系统是Debian或Ubuntu系统，可不用安装内核，直接输入数字4启动bbr原版加速。）

以安装暴力BBR魔改版加速为例，我们先安装对应的内核，输入数字1

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/vultr/newbbr2.jpg)

内核安装完成后，输入y进行重启，重启才能让内核生效

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/vultr/newbbr3.jpg)

重启完成后，输入数字6来启动暴力BBR魔改版加速

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/vultr/newbbr4.jpg)

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/vultr/newbbr5.jpg)

输入./tcp.sh查看最终是否启动成功。

如果想换一个加速，输入数字9进行卸载加速，然后进行同样的操作，安装内核再安装对应内核的加速即可。

**注意：如果在安装内核环节出现这样一张图，注意选择NO**

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/vultr/newbbr6.jpg)

***

【客户端下载及使用方法】

windows电脑系统推荐使用v2rayN客户端，最好用v2rayN最新版。

**注意**：第一次使用v2rayN客户端时，需要安装最新版NET Framework ，不然无法正常运行，[微软官网](https://dotnet.microsoft.com/zh-cn/download/dotnet-framework/net48)下载。

windows v2rayN 客户端：[github最新版下载](https://github.com/2dust/v2rayN/releases/latest) (下载带core的文件) [github镜像下载](https://dgithub.xyz/2dust/v2rayN/releases/latest) (下载带core的文件)

Mac客户端 v2rayU 客户端：[github最新版下载](https://github.com/yanue/V2rayU/releases) [github镜像下载](https://dgithub.xyz/yanue/V2rayU/releases)

Linux客户端 Qv2ray 客户端：[github最新版下载](https://github.com/lhy0403/Qv2ray/releases)  [github镜像下载](https://dgithub.xyz/lhy0403/Qv2ray/releases) 

安卓v2rayNG 客户端：[github最新版下载](https://github.com/2dust/v2rayNG/releases) [github镜像下载](https://dgithub.xyz/2dust/v2rayNG/releases)


iOS：[没有美区AppleID的翻墙教程](https://github.com/Alvin9999/new-pac/wiki/%E8%8B%B9%E6%9E%9C%E6%89%8B%E6%9C%BA%E7%BF%BB%E5%A2%99%E8%BD%AF%E4%BB%B6) [iOS注册美区Apple ID教程](https://github.com/Alvin9999/new-pac/wiki/iOS%E6%B3%A8%E5%86%8C%E7%BE%8E%E5%8C%BAApple-ID%E6%95%99%E7%A8%8B) 

**软件代理设置**：

![](https://cdn.jsdelivr.net/gh/Alvin9999/pac2/softimag/v2rayn001.jpg)

windows系统打开v2rayN软件，在软件的底部，选择“自动配置系统代理”，路由可选择“全局(Global)”。全局(Global)模式：所有网站通过节点服务器代理上网。


***

**注意事项**：

1、电脑如果使用V2rayN客户端，最好用v2rayN最新版，至少使用6.43及以上版本，不然节点可能无法使用。因为脚本搭建的时候服务器用的是最新版的服务端,所以客户端的版本太老的话可能就不兼容。其它操作系统的客户端也一样,也最好用最新版。v2rayN最新版下载地址：https://github.com/2dust/v2rayN/releases

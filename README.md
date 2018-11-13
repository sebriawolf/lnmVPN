# 安装步骤(本文仅针对centos/redhat发行版，其他版本自行测试)

1. 安装初始化环境 python >=2.7 ;推荐lnmos定制版本
[关闭selinux] vim /etc/selinux/config
rpm -i python27-2.7.15-lnmos.rpm


2. 安装pip环境并安装相关python组件模块
MySQL服务: mysql-server mysql-devel MySQL-Python
VPN服务: ocserv openconnect epel-release[yum第三方源]
证书组件: gnutls-utils
yum install gcc mysql-server mysql-devel ocserv openconnect epel-release gnutls-utils
程序扩展包: pip install -r requirements.txt

3. 创建数据库并恢复数据模版
[创建数据库]
[恢复数据模版]

4. 正式运行程序
[程序调试]：python main.py 
[后台运行]: startweb.sh restart

备注：程序启动将自动接管网络接口配置、DNS服务、DHCP服务等相关，建议关闭系统中涉及到的相关程序，以免相互冲突。


## 项目截图
### 系统管理
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/文件管理.png)
### 网络配置
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/进程监控-详细.png)
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/进程监控-总览.png)
### UTM防护
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/计划任务.png)
### VPN配置
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/SSH.png)
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/SSH链接.png)
### 日志审计
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/资源监控.png)
### 帮助文档
![其余界面](https://github.com/cksgf/WebFileManager/blob/master/readme/资源监控.png)

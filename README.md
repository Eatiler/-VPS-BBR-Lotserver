【vps】安装SSR+BBR/Lotserver魔改加速<br>
=========================================
#ShadowsocksR+优化加速一键安装脚本(8K youtube无压力)<br>

安装【秋水逸冰】的ShadowsocksR一键安装脚本
原地址:https://shadowsocks.be/9.html

使用方法：
使用root用户登录，运行以下命令：

```

wget --no-check-certificate https://raw.githubusercontent.com/teddysun/shadowsocks_install/master/shadowsocksR.sh
chmod +x shadowsocksR.sh
./shadowsocksR.sh 2>&1 | tee shadowsocksR.log

```

<br>

##默认配置：
```
服务器端口：自己设定（如不设定，默认从 9000-19999 之间随机生成）
密码：自己设定（如不设定，默认为 teddysun.com）
加密方式：自己设定（如不设定，默认为 aes-256-cfb）
协议（Protocol）：自己设定（如不设定，默认为 origin）
混淆（obfs）：自己设定（如不设定，默认为 plain）

```


```
安装完成后，脚本提示如下：

Congratulations, ShadowsocksR server install completed!
Your Server IP        :your_server_ip
Your Server Port      :your_server_port
Your Password         :your_password
Your Protocol         :your_protocol
Your obfs             :your_obfs
Your Encryption Method:your_encryption_method

Welcome to visit:https://shadowsocks.be/9.html
Enjoy it!

```
###卸载方法：
<br>
使用 root 用户登录，运行以下命令(谷歌云使用 ` sudo -i ` )：

```
./shadowsocksR.sh uninstall

```
本脚本安装完成后，已将 ShadowsocksR 自动加入开机自启动。

使用命令：
```
启动：/etc/init.d/shadowsocks start
停止：/etc/init.d/shadowsocks stop
重启：/etc/init.d/shadowsocks restart
状态：/etc/init.d/shadowsocks status

配置文件路径：/etc/shadowsocks.json
日志文件路径：/var/log/shadowsocks.log
代码安装目录：/usr/local/shadowsocks
```

网络优化加速一键脚本
------------------

支持系统
Centos 6+ / Debian 7+ / Ubuntu 14+
BBR魔改版不支持Debian 8

```
wget -N --no-check-certificate "https://raw.githubusercontent.com/chiakge/Linux-NetSpeed/master/tcp.sh"
chmod +x tcp.sh
./tcp.sh
```

根据自己需求操作，重启后再使用 ` ./tcp.sh  ` 命令接着操作

# 测试网卡
```
1. 给对接的82599网口配置ip:
   切换到root用户下
   a端口:ifconfig -s eth6 192.168.1.xxx 255.255.255.0
   b端口:ifconfig -s eth6 192.168.1.xxx 255.255.255.0
2. 关闭以太网口:ifconfig eth0 down
3. ping对端ip:ping -I eth6 192.168.1.xxx
```

# 测试网速
```
1. 给对接的82599网口配置ip:
   切换到root用户下
   a端口:ifconfig -s eth6 192.168.1.xxx 255.255.255.0
   b端口:ifconfig -s eth6 192.168.1.xxx 255.255.255.0
2. 关闭以太网口:ifconfig eth0 down
3. 下发scp命令从服务器拷贝一个发行版压缩文件:scp fangyuanzheng@192.168.1.107:~/tftp/ubuntu/Ubuntu_ARM64.tar.gz .
```

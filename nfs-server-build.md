# Install nfs server 
```
$ sudo apt-get install nfs-kernel-server ---ubuntu
$ sudo yum install nfs-utils rpcbind
```
# Config exports
```
$ vi /etc/exports
在最后添加:
/<服务器共享目录> *(rw,sync,no_root_squash)
```
# Restart nfs service(修改配置后的必须操作)
```
$ sudo service nfs-kernel-server restart
```
# Client mount server
```
$ sudo mount -t nfs -o nolock <serverip>:/<服务器共享目录> /home/<本地挂载目录>
```


# 使用nfs

## 服务端启动

```
./osnfs /bigant  2049
```
## 客户端挂载
```
mount -o port=2049,mountport=2049,nfsvers=3,noacl,tcp,nolock -t nfs \
192.168.0.200:/bigant /home/im_user/im_server/im_server/data1
```
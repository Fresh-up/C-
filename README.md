# ChatServer

# 编译要求

需要GCC/G++版本在7.0以上，需要先安装boost库，再安装muduo网络库

为了实现离线消息订阅的功能，必须安装redis

为了实现负载均衡，需要安装nginx

且需要手动配置MySQL，创建数据库名chat，创建5张表: 

*   allgroup
*   friend
*   groupuser
*   offlinemessage
*   user

环境搭建好后便可以进入ChatServer文件夹，依次执行命令

```powershell
cmake .
make
```

生成的可执行文件在bin目录

```powershell
./ChatServer 127.0.0.1 6000 # 开启服务器，端口不一定6000，可以自己设定
./ChatClient 127.0.0.1 6000 # 在另一终端开启客户端
```

# 7.2添加功能

1.   客户端显示群组列表命令
2.   客户端显示好友列表命令

# 4.27完成的功能

1. 群组业务
2. 客户端开发
   1. 首页功能
   2. 添加好友和聊天
   3. 离线消息表设计
   4. 群组
   5. 群组聊天功能
   6. 用户注销


##### 命令

geth attach

可以让geth连接上 mist所开启的节点 还是反过来？

并且开启geth控制台





Mac 安装mist的dmg安装包



==mist连接私有链节点==



> 连接ganache节点

定位到/Applications/Mist.app/Contents/MacOS 下

命令行运行

./Mist --rpc http://127.0.0.1:7545

或者在任意目录运行

/Applications/Mist.app/Contents/MacOS/Mist --rpc http://127.0.0.1:7545

即可连接上ganache私链节点



mist多重签名钱包设置 0.11.1最新版本 ganache可能报错 不支持personal_signature方法

用户0.10版本试试



> 连接geth节点

先用geth命令启动geth私有链

在控制台信息中的IPC endpoint opened可看到url=xxx

路径 /Users/superman285/Desktop/PrivateChain/data0/geth.ipc 我的路径示例

然后./Mist --rpc /Users/superman285/Desktop/PrivateChain/data0/geth.ipc

即可连接上geth私有节点





> 非常好用的工具

Mist打开开发者界面

控制台可以直接看web3对象 Web3构造函数

自带web3 非常实用！



mist的开发者界面 类似geth控制台 可以打命令测试

先连上测试账户 然后可以打web3命令看一些信息
# React-Native成长日记
本日记用于记录自己在使用react-native开发过程中遇到的各种问题、解决方案、思考总结等等
正不断更新中，如有错误，希望大家指正。

# 目录
* [启动](#启动)
## 启动
首先，根据文档用create-react-native-app来新建工程；并且，用Expo客户端扫描二维码后运行app
其次，扫描之后，可能会发现Expo客户端不能加载出app，并提示“Uncaught Error: Java.net,sockettimeoutException: failed to connect to after 10000ms”
在网上查了一大圈，据说这是create-react-native-app的一个bug，解决方案如下：
1、关闭windows防火墙
2、在电脑，在“网路设定->修改适配器设置”中，disable所有的virtual network（除wifi之外的）。 因为这些网络存在，可能会让create-react-native-app启动的服务在这些网络，而不是wifi的网络中。

# 网络通信系统平台
# 前言说明
* 这是一个由个人开发的网络通信系统平台，主要使用TCP、UDP、HTTP、SMTP等网络协议进行不同子功能的开发，使用了Qt框架，多线程，C++等技术。此项目由个人开发完成，代码总行数约一万行左右。
* 项目主要有四大功能模块：聊天模块、GIF录屏模块、天气系统模块、发送邮件模块。
# 开发环境
Qt 5.15.2 + MinGW  
Windows 10
# 主界面介绍
* 采用Qt的QSS样式设置布局，并使用了自定义控件实现相应的效果。  
* 项目支持一键换主题颜色功能，可点击相应的功能按钮实现对应的功能。
![image](https://github.com/SjhTT/-/assets/147903319/e63780c2-816e-4c71-bb01-c6e8498d6095)
# 聊天模块
* 通过UDP进行广播通信，使用TCP进行文件传输，并采用多线程技术进行文件传输功能的实现，以确保在传输大文件时不会堵塞UI界面的使用。  
* 可支持富文本模式发送信息，支持自定义区域截屏功能，支持导出聊天记录功能，支持同时存在多个聊天房间并各自进行通信的功能，支持用户房间收到的新信息进行缓存功能。  
* 用户可在聊天室里点击加入群聊，即可快速进入群聊功能，并可在在线用户列表中查看已加入聊天室的所有用户IP、主机名、用户名等，可以实现快速传输文件以及发送信息通信的功能。  
* 也可在私聊功能中通过输入房间号的方式加入房间建立私聊，一个私聊房间最多同时存在两人，也可以自定义群聊。  
* 为每个房间创建一个房间列表，可显示头像，房间号，对方用户名等功能。
# GIF录屏模块
* 采用屏幕捕捉技术捕捉屏幕内容，将捕捉到的内容进行编码、解码操作，并对动画使用压缩算法进行压缩，最终转成GIF格式的动画。  
* 可设置录制屏幕的宽高，并支持直接通过窗口右下角拉动改变窗口大小。  
* 可设置录制的帧数。  
* 录制区域可自由拖动选择。
# 天气系统模块
* 从国家气象局提供的 API  接口中获取 JSON  数据，使用 Qt  提供的类来解析 JSON  数据。  
* 发送 HTTP  请求，获得天气数据,自行绘制温度曲线和查看当前天气，所有天气图表都有显示。  
* 可以搜索国内所有城市天气预报,查看感冒指数、空气质量、未来6天空气、风力风向和最高最低温度。  
# 发送邮件模块
* 使用SMTP协议进行发送邮件功能，支持用户使用七种不同的邮箱服务发送邮件。  
* 通过多线程处理发送邮件功能。





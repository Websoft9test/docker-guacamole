## Guacamole

通过web实现无客户端连接远程图形化桌面

#### 架构图

![image](https://user-images.githubusercontent.com/43192516/162339222-9f0f80d6-f541-497c-a089-d54e1336a338.png)

Guacamole是一个tomcat实现的web程序，它本身不了解vnc，rdp协议，它和guacd通过用自己的协议通信。guacd 才是 Guacamole 的核心，guacd 也不理解任何特定的远程桌面协议。但是它接受web端连接请求，通过加载插件来实现远程连接。



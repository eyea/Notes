## 三次握手
客户端和服务端进行连接时要进行三次握手
第一次握手： 客户端发送一个SYN=1报文给服务端，不能携带数据
第二次握手： 服务端收到客户端发来的SYN报文后，发送一个SYN和ACK报文响应给客户端
第三次握手： 当客户端收到了服务端发来的报文，向服务端发送一个ACK报文表示已接收到报文。

## 三次握手的原因？

确认双方都有请求和响应的能力。

## 三次握手过程都可以携带数据吗？
第一次第二次不行， 第三次可以
假设第一次可以携带数据，攻击者在SYN中放入大量数据，服务器要花费很多精力来接收报文。

第三次可以的原因是已经确认服务端接收发送能力正常，客户端也已经处于建立状态了。



https://juejin.im/post/5ccd0dfc6fb9a0324a08bb73
# Web

## 单点登录
* [CAS实现SSO单点登录原理](http://www.coin163.com/java/cas/cas.html)

## 负载均衡
* [Keepalived 虚拟IP技术 ip地址漂移技术](https://www.cnblogs.com/myseries/p/11409895.html)
> VIP是虚拟IP，可以在不同主备服务器之间漂移（依赖TCP/IP的ARP协议）。

## Nginx
* [Nginx 相关介绍(Nginx是什么?能干嘛?)](https://www.cnblogs.com/wcwnina/p/8728391.html)
* [你真的了解如何将 Nginx 配置为Web服务器吗](https://lufficc.com/blog/configure-nginx-as-a-web-server)
* [用了10多年的 Tomcat 居然有bug，这能忍？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486521&idx=1&sn=b4652b03579a43b5ab9f243653ffd114)
> tomcat 遵循 RFC1-1034 的规范，不允许带有下划线的Host（domain name）。  
https://www.ietf.org/rfc/rfc1034.txt  
可通过在 Nginx 中配置``proxy_set_header HOST $host``解决。

* [除了负载均衡，Nginx还可以做很多，限流、缓存、黑白名单等](https://mp.weixin.qq.com/s?__biz=MzU0MzQ5MDA0Mw==&mid=2247486150&idx=1&sn=a85f3352d6bfebe040e03b289ad39eb1)

## 前端
* [如何设计好的RESTful API](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483661&idx=1&sn=048af6543c7baf6cefa691f80587b4c3)
* [RESTful API设计规范](https://www.cnblogs.com/mayite/p/9798913.html)
* [干掉状态：从session到token](http://mp.weixin.qq.com/s?__biz=MzAxOTc0NzExNg==&mid=2665513566&idx=1&sn=a2688cadbe9c8042ff1abbdf04a8bd5e)
* [JWT & JWS & JWE](https://gblog.sherlocky.com/jwt/)
* [Web登录其实没那么简单](https://www.cnblogs.com/letcafe/p/loginSecurity.html)
* [80% 应聘者都不及格的 JS 面试题](https://juejin.im/post/58cf180b0ce4630057d6727c)

## HTTP/HTTPS, TCP/IP
* [HTTP灵魂拷问，你了解你的每次请求吗？](https://mp.weixin.qq.com/s/mmiRIb-nQLQKVGFYUYYbHQ)
  > RSA 算法不具备前向安全性，而 ECDHE 具备，因此在 TLS1.3（1-RTT握手） 中彻底取代了RSA（一次破解并不影响历史信息的性质也叫前向安全性）。

  > CORS 请求中的非简单请求，会先发送一个**预检请求**，预检请求的方法是：``OPTIONS``.

* [TCP为啥要3次握手和4次挥手？握两次不行吗？](https://www.cnblogs.com/qdhxhz/p/8470997.html)
* [数据加密、HTTPS、线上充值原理？看我就够啦-肥朝](https://www.jianshu.com/p/2cb959529c96)
* [再谈HTTPS](https://zhuanlan.zhihu.com/p/75461564)
  > RSA -> ECC (椭圆曲线加密)
* [TCP长连接和心跳那些事](https://mp.weixin.qq.com/s/U5SQkaCI2DI6WiaRYVpN2g)
* [面试官问一个 TCP 连接可以发多少个 HTTP 请求？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486325&idx=1&sn=1dd32634cc92402934e85a43691c1011)
* [从输入url到页面展示到底发生了什么](https://www.cnblogs.com/xianyulaodi/p/6547807.html)

* [CentOS7 Certbot 自动更新 Let's Encrypt SSL 证书(Nginx,https)](https://halo.sherlocky.com/archives/centos7-certbot-nginx-ssl)

## HTTP3 QUIC协议
* ![](https://ghost.oss.sherlocky.com/halo/http3_1589801866231.png)

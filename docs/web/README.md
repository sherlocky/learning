# Web
## 图解网络
* [图解网络](https://www.xiaolincoding.com/network/)

## 五元组
五元组是一个通信术语，英文名称为five-tuple,或5-tuple，通常指由**源Ip (source IP), 源端口(source port),目标Ip (destination IP), 目标端口(destination port),4层通信协议 (the layer 4 protocol)**等5个字段来表示一个会话。

**五元组规则包含：源IP地址、源端口、目的IP地址、目的端口、传输层协议。**

> 通常使用5元组来标识一个数据包属于哪个会话，在数据包查重和流量对比时会使用较多，在网络分析领域也经常会涉及到。
> 类似的还有：
> 4元组即用4个维度来确定唯一连接，这4个维度分别是源Ip (source IP), 源端口(source port),目标Ip (destination IP), 目标端口(destination port)。
> 7元组即用7个字段来确定网络流量，即源Ip (source IP), 源端口(source port),目标Ip (destination IP), 目标端口(destination port),4层通信协议 (the layer 4 protocol),服务类型(ToS byte)，接口索引(Input logical interface (ifIndex))

### 一个端口多个连接
- 一个端口能建立多个TCP连接（五元组不同即可），一个端口同一时间只能bind给一个SOCKET。就是同一时间一个端口只可能有一个监听线程(监听listen之前要bind)。
- UPD本身就是无连接的。所以不存在什么多个UDP连接。只是，服务端接收UDP数据需要bind一个端口。一个SOCKET只能绑定到一个端口。

## 性能&高并发
* [理解 QPS、TPS、RT、并发数、吞吐量...](https://mp.weixin.qq.com/s/v0r-bZ_KVT9dLV_r7bNbjA)
> QPS = 并发数 / RT  
> 并发数 = QPS * RT  
> 最佳线程数 = RT/CPU Time * CPU核心数 * CPU利用率  
> 最大QPS = 最佳线程数 * 单线程QPS = (RT/CPU Time * CPU核心数 * CPU利用率)*（1/RT) = CPU核心数 * CPU利用率 / CPU time  
* [如何排查系统的性能瓶颈点？](https://mp.weixin.qq.com/s/PIs6ZVDzZChY1n3uEKnNKg)

## 服务端
* [服务端如何安全存储密码？](https://mp.weixin.qq.com/s?__biz=MzA5NDIzNzY1OQ==&mid=2735616885&idx=1&sn=f7b605c1d31a16e16150b8da43e22a4e)

## 单点登录
* [CAS实现SSO单点登录原理](http://www.coin163.com/java/cas/cas.html)
* [统一身份认证（CAS）的工作流程](https://www.jianshu.com/p/35ba532780ec)
* [apereo/cas](https://github.com/apereo/cas)
* [OAuth2.0 的四种授权方式](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247487003&idx=1&sn=47cd6b064a7fc3b3df8f6f4c3f7669a7&scene=21)
* [OAuth2.0实战--用三方 Github 做授权登录](https://mp.weixin.qq.com/s/KzWE4EtZ6F4_-2fYnVA5QA)

## 权限认证框架
* [Sa-Token 一个轻量级 java 权限认证框架](https://sa-token.dev33.cn/index.html)
> 登录认证、权限认证、分布式Session会话、微服务网关鉴权、单点登录、OAuth2.0、踢人下线、Redis集成、前后台分离、记住我模式、模拟他人账号、临时身份切换、账号封禁、多账号认证体系、注解式鉴权、路由拦截式鉴权、花式token生成、自动续签、同端互斥登录、会话治理、密码加密、jwt集成、Spring集成、WebFlux集成...

## 负载均衡
* [Keepalived 虚拟IP技术 ip地址漂移技术](https://www.cnblogs.com/myseries/p/11409895.html)
> VIP是虚拟IP，可以在不同主备服务器之间漂移（依赖TCP/IP的ARP协议）。

## Tomcat
* [用了10多年的 Tomcat 居然有bug，这能忍？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486521&idx=1&sn=b4652b03579a43b5ab9f243653ffd114)
> tomcat 遵循 RFC1-1034 的规范，不允许带有下划线的Host（domain name）。  
https://www.ietf.org/rfc/rfc1034.txt  
可通过在 Nginx 中配置``proxy_set_header HOST $host``解决。
* [web.xml中<security-constraint>安全认证标签说明](https://www.cnblogs.com/xiohao/p/10935004.html)
  > Tomcat 可使用在 web.xml 中配置 <security-constraint> 解决不安全的 HTTP 方法安全漏洞
* [spring boot使用内嵌的tomcat解决不安全的HTTP方法安全漏洞](https://www.jianshu.com/p/8eb6b8ea4371)

## Nginx
* [Nginx 相关介绍(Nginx是什么?能干嘛?)](https://www.cnblogs.com/wcwnina/p/8728391.html)
* [你真的了解如何将 Nginx 配置为Web服务器吗](https://lufficc.com/blog/configure-nginx-as-a-web-server)

* [除了负载均衡，Nginx还可以做很多，限流、缓存、黑白名单等](https://mp.weixin.qq.com/s?__biz=MzU0MzQ5MDA0Mw==&mid=2247486150&idx=1&sn=a85f3352d6bfebe040e03b289ad39eb1)
* [Nginx配置中一个不起眼字符"/"的巨大作用，失之毫厘谬以千里](https://zhuanlan.zhihu.com/p/100577578)
* [Nginx状态监控及日志分析](https://www.jianshu.com/p/59ed801213ca)
* [面试官：我想用Nginx提升系统10倍性能，你有哪些建议?](https://mp.weixin.qq.com/s?__biz=MzU0MzQ5MDA0Mw==&mid=2247492351&idx=1&sn=ed34731df8e608a5f921dc46ea6593b1)

## 前端
* [如何设计好的RESTful API](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483661&idx=1&sn=048af6543c7baf6cefa691f80587b4c3)
* [RESTful API设计规范](https://www.cnblogs.com/mayite/p/9798913.html)
* [干掉状态：从session到token](http://mp.weixin.qq.com/s?__biz=MzAxOTc0NzExNg==&mid=2665513566&idx=1&sn=a2688cadbe9c8042ff1abbdf04a8bd5e)
* [JWT & JWS & JWE](https://gblog.sherlocky.com/jwt/)
* [Web登录其实没那么简单](https://www.cnblogs.com/letcafe/p/loginSecurity.html)
* [Token多平台身份认证架构设计思路](https://mp.weixin.qq.com/s/aQs3IbhfBAaSfqBLbwfnkw)
  > http://cnblogs.com/beer/p/6029861.html
* [80% 应聘者都不及格的 JS 面试题](https://juejin.im/post/58cf180b0ce4630057d6727c)

## HTTP/HTTPS, TCP/IP
* [TCP协议面试灵魂10问，建议收藏~](https://mp.weixin.qq.com/s/B-Uc61AJLnVaFiG909RN0g)
* [HTTP灵魂拷问，你了解你的每次请求吗？](https://mp.weixin.qq.com/s/mmiRIb-nQLQKVGFYUYYbHQ)
  > RSA 算法不具备前向安全性，而 ECDHE 具备，因此在 TLS1.3（1-RTT握手） 中彻底取代了RSA（一次破解并不影响历史信息的性质也叫前向安全性）。

  > CORS 请求中的非简单请求，会先发送一个**预检请求**，预检请求的方法是：``OPTIONS``.

* [TCP为啥要3次握手和4次挥手？握两次不行吗？](https://www.cnblogs.com/qdhxhz/p/8470997.html)
* [数据加密、HTTPS、线上充值原理？看我就够啦-肥朝](https://www.jianshu.com/p/2cb959529c96)
* [再谈HTTPS](https://zhuanlan.zhihu.com/p/75461564)
  > RSA -> ECC (椭圆曲线加密)
* [TCP长连接和心跳那些事](https://mp.weixin.qq.com/s/U5SQkaCI2DI6WiaRYVpN2g)
* [服务端推送对比：``客户端轮询`` vs ``服务端轮询`` vs ``WS`` vs ``SEE``](https://mp.weixin.qq.com/s/Z3K1u_jF_UQBgxRuFouEcg)
* [面试官问一个 TCP 连接可以发多少个 HTTP 请求？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486325&idx=1&sn=1dd32634cc92402934e85a43691c1011)
* [服务端 TCP 连接的 TIME_WAIT 问题](http://ningg.top/computer-basic-theory-tcp-time-wait/)
* [浏览器从输入url到页面展示到底发生了什么](https://www.cnblogs.com/xianyulaodi/p/6547807.html)
* [浏览器键入网址url后，期间发生了什么？](https://mp.weixin.qq.com/s/I6BLwbIpfGEJnxjDcPXc1A)

* [CentOS7 Certbot 自动更新 Let's Encrypt SSL 证书(Nginx,https)](https://halo.sherlocky.com/archives/centos7-certbot-nginx-ssl)

### CLOSE_WAIT
* [浅谈CLOSE_WAIT](https://cloud.tencent.com/developer/article/1918110)

## WebSocket
* [WebSocket API安全风险解读](https://www.anquanke.com/post/id/289510)

### CORS
  * [后端工程师的「跨域」之旅](https://mp.weixin.qq.com/s/dgwyeTyE7tmLzC_iyNh7Hw)

#### Private Network Access
  * [cors-rfc1918](https://wicg.github.io/private-network-access/)
  * [2021新规范-私有网络请求（Private Network Access）](https://juejin.cn/post/7026130384001859615)
  * [chrome 更新跨域规则，将对网站造成影响](https://juejin.cn/post/7025485128436547615)
  
### SNI
 * [java使用httpclient调用多虚拟主机https接口报错问题](https://stackoverflow.com/questions/39762760/javax-net-ssl-sslexception-certificate-doesnt-match-any-of-the-subject-alterna)
 > javax.net.ssl.SSLException: Certificate doesn't match any of the subject alternative names
 > 使用了 httpclient 4.5.1版本，该版本处理 SNI 时存在bug，需要更新到4.5.3+修复
 * [HTTPS 深入浅出 - 什么是 SNI？](https://blog.csdn.net/firefile/article/details/80532161)
 * [SNI(Server Name Indication)](https://blog.csdn.net/makenothing/article/details/53292335)

## 安全
* [技术中台之移动平台安全架构设计](https://mp.weixin.qq.com/s/WGXoARbfO9sH8YA8aS3WXg)
* [接口签名](https://www.jianshu.com/p/e2d362ede89f)

### HTTPS 双向认证
* [HTTPS双向认证（Mutual TLS authentication)](https://help.aliyun.com/document_detail/160093.html)
* [Https单向认证和双向认证](https://blog.csdn.net/duanbokan/article/details/50847612)
* [扯一扯HTTPS单向认证、双向认证、抓包原理、反抓包策略](https://juejin.cn/post/6844903809068564493)

## SSL
* [本地https解决方案](https://www.jianshu.com/p/7cb5c2cffaaa)
  > https://github.com/FiloSottile/mkcert

### ``TLS`` VS ``DTLS``
  > ![](https://ghost.oss.sherlocky.com/halo/TLS_DTLS.png)
  
## HTTP3 
* [HTTP/3 QUIC协议](https://mp.weixin.qq.com/s/mHPEOho5F1pmNSWUAXQ9QA)
  > QUIC（Quick UDP Internet Connections，快速 UDP 网络连接
  > ![QUIC协议](https://ghost.oss.sherlocky.com/halo/http3_1589801866231.png)
  > [HTTP/3 强势来袭](https://www.xiaolincoding.com/network/2_http/http3.html)
* [在Nginx中支持HTTP3.0/QUIC](https://zhuanlan.zhihu.com/p/159100819)
* [NGINX官方对QUIC和HTTP/3的支持的技术预览介绍](https://www.nginx.com/blog/introducing-technology-preview-nginx-support-for-quic-http-3/)
  > 支持QUIC的Nginx分支：https://hg.nginx.org/nginx-quic/shortlog/quic ，基于mainline 1.19.x 版本开的分支，目前处于Beta版质量，不应用于生产。
  > 以及部署说明：https://quic.nginx.org/readme.html
  > 测试你的站点是否支持 quic 服务：https://http3check.net/

## DNS
> 美国已经利用先发优势主导的根服务器治理体系控制全球互联网长达30年了，根服务器负责互联网最顶级的域名解析，被称为互联网的“中枢神经”。
> 由美国一手构建起来的IPv4体系，在全球部署13台根服务器，唯一主根部署在美国，其余12台辅根中9台在美国、2台在欧洲、1台在日本。
>
> 下一代互联网国家工程中心牵头发起的“雪人计划”在全球完成25台IPv6(互联网协议第六版)根服务器架设。
> 中国部署了其中的4台，由1台主根服务器和3台辅根服务器组成。打破了中国过去没有根服务器的困境。
- IPv4 DNS
  - Google 公共 DNS
    - ``8.8.8.8``
    - ``114.114.114.114``
  - 腾讯 ``119.29.29.29``
  - 阿里
    > 24年9月30日免费版开始限速了
    - ``223.5.5.5``
    - ``223.6.6.6``
- [IPv6 DNS](https://halo.sherlocky.com/archives/ipv6#34-ipv6-dns)
- [DoH 与 DoT 说明](https://halo.sherlocky.com/archives/ipv6#33-doh-%E4%B8%8E-dot-%E8%AF%B4%E6%98%8E)

## ``IPv4`` VS ``IPv6``
* [为什么 IPv6 难以取代 IPv4](https://mp.weixin.qq.com/s/Aut6e6duxkCZ4f4mZcD2-g)
* [【博客】IPv6](https://halo.sherlocky.com/archives/ipv6)
* [IPv6 工具箱使用](https://ipw.cn/doc/)

## gor
* [gor实现线上HTTP流量复制压测引流](https://www.cnblogs.com/qmfsun/p/11598763.html)
* [【github】buger/goreplay](https://github.com/buger/goreplay)

## 网络诊断调试
* [Corgi - 打印 HTTP 请求](https://github.com/ddrpa/corgi)
* [Traefik's Whoami：一款轻巧且强大的网络调试工具](https://github.com/traefik/whoami)
  > 支持Docker部署
  > 在软件开发和运维中，理解请求在网络中的流动是至关重要的。这款小巧但功能强大的服务提供了一个简单的API接口，用于展示当前连接的信息，帮助开发者进行网络和负载均衡器的调试。
  > Whoami服务简单地响应HTTP请求，返回客户端的IP地址、User-Agent、服务器时间等信息，这对于诊断和测试网络配置非常有用。

# 微服务/分布式
* [dubbo高并发服务，每次重启都大量超时！](https://mp.weixin.qq.com/s?__biz=MzU5ODUwNzY1Nw==&mid=2247484742&idx=1&sn=fb179195b52762a35f804ec5cd406c9e)
* [Dubbo 学习1——Service自定义异常捕获不到问题](https://gblog.sherlocky.com/dubbo1/)
* [Dubbo 学习2——SPI 扩展机制](https://my.oschina.net/j4love/blog/1813040)  
* [DUBBO原理、应用与面经总结](https://www.jianshu.com/p/292fcdcfe41e)
* [dubbo源码解析-连载-肥朝](https://www.jianshu.com/nb/6137390)
* [dubbo源码解析-zookeeper订阅](https://www.jianshu.com/p/73224a6c07bb)
* [dubbo源码解析-服务暴露原理](https://www.jianshu.com/p/60a9263f2ee2)
  > Dubbo 一个服务可能既是Provider,又是Consumer,因此就存在自己调用自己服务的情况,就有了本地暴露服务的这个设计:
  - 本地暴露：是暴露在 JVM 中，不需要网络通信。
  - 远程暴露：是将ip，端口等信息暴露给远程客户端，调用时需要网络通信。

* [分布式数据缓存中的一致性哈希算法（有哈希环）](https://mp.weixin.qq.com/s?__biz=Mzg2NjE5NDQyOA==&mid=2247483762&idx=1&sn=f377cf428ac99d9c940d7e4c485de42e)
* [这样讲API网关，你应该能明白了吧](https://mp.weixin.qq.com/s?__biz=MzIxNjA5MTM2MA==&mid=2652436269&idx=2&sn=29476be3045bac709d72e8d6b0f7ea55)
* [谈谈高并发系统的限流](https://www.cnblogs.com/haoxinyue/p/6792309.html)

## 一致性 HASH
* [图解一致性哈希算法](https://mp.weixin.qq.com/s/3QO59gjmByj9zCk2VpwSeA)
  > - Hash 环
  > - 顺时针
  > - 数据倾斜
  > - 节点雪崩
  > - 虚拟节点
* [一致性哈希算法（Consistent Hashing）](//halo.sherlocky.com/archives/yi-zhi-xing-ha-xi-suan-fa-consistent-hashing)

## 分布式ID
* [一口气说出 9种 分布式ID生成方式，面试官有点懵了](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247483785&idx=1&sn=8b828a8ae1701b810fe3969be536cb14)
* [发号器-分布式ID生成系统](https://mp.weixin.qq.com/s?__biz=MzIwODA4NjMwNA==&mid=2652899291&idx=1&sn=3dd7b9224a7cead4284d1f72590a7fcc) 
* [9种分布式ID生成之美团（Leaf）实战](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247483889&idx=1&sn=35b0eb32de3e63c013585ef1db5d3076)
* [分布式ID之滴滴（Tinyid）](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247483948&idx=1&sn=4a06498011aaa71b0565d89e4d4f4e64)

## Zookeeper
> ZooKeeper主要服务于分布式系统，可以用ZooKeeper来做：  
统一配置管理、统一命名服务、分布式锁、集群管理。

* [zookeeper的一些基本的概念](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247484003&idx=1&sn=be5633aaf3346044ea9c2c5f92057d93)

* [脑裂是什么？Zookeeper是如何解决的？](https://juejin.im/post/5d36c2f25188257f6a209d37)
  > 使用(选举)过半机制，避免产生脑裂(核心在于，必须**超过半数**，等于半数都不行！)。

* [可能是全网把 ZooKeeper 概念讲的最清楚的一篇文章](https://mp.weixin.qq.com/s/rMl60YKnSVL5GfkXU8p9Ow)
  > ![](https://ghost.oss.sherlocky.com/8/de/274eb6351bdf85a64e4ce1a4b9f65.png)
  > ![](https://ghost.oss.sherlocky.com/8/1c/b1ddd7ae9abdda6d7d6b1c1878b60.jpg)

## 分布式事务
* [分布式事务（2PC、3PC、TCC）](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247483940&idx=1&sn=d3643c25b910be46d253238c725dd163)
* [**消息队列**分类下也有相关文章](mq/?id=消息队列)

* [微服务架构下的事务一致性保证](https://mp.weixin.qq.com/s?__biz=MzI3MzEzMDI1OQ==&mid=2651815502&idx=1&sn=ba36068070be434cbbd48f594f697532)
  
## 分布式任务
* [6大分布式定时任务对比](https://blog.csdn.net/u012394095/article/details/79470904)

## 分布式监控（调用链）
* [分布式调用链调研（pinpoint,skywalking,jaeger,zipkin等对比）](https://my.oschina.net/u/3770892/blog/3005395)
* [APM和调用链跟踪](http://devops.weiminginfo.com/yunwei/apm/1522.html)

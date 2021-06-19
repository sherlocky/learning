# 缓存

## 缓存算法
* [LFU的基本原理与实现](https://www.cnblogs.com/wyq178/p/11790015.html)

## 本地缓存
* [【本地缓存之王】Caffeine高性能设计剖析](https://albenw.github.io/posts/a4ae1aa2/)
* 本地缓存不放敏感变更数据，Maybe 可以通过配置中心异步通知的方式更新本地缓存？

## Redis
* [《吊打面试官》系列- Redis基础](https://juejin.im/post/5db66ed9e51d452a2f15d833)
* [Redis-避免缓存穿透的利器之BloomFilter](https://juejin.im/post/5db69365518825645656c0de)
* [《吊打面试官》系列-缓存雪崩、击穿、穿透](https://juejin.im/post/5dbef8306fb9a0203f6fa3e2)
* [《吊打面试官》系列-Redis哨兵、持久化、主从、手撕LRU](https://juejin.im/post/5dc3a9fbf265da4d3c072eab)
* [《吊打面试官》系列-Redis终章](https://juejin.im/post/5dc850b4e51d452c2308ee27)
* [《吊打面试官》系列-Redis常见面试题（带答案）](https://juejin.im/post/5dcaebea518825571f5c4ab0)
* [探秘 Redis 中键的自动过期功能](https://mp.weixin.qq.com/s?__biz=MzA3NDcyMTQyNQ==&mid=2649263256&idx=1&sn=f5dbd5610d197c568a254bcbc973880e)
* [解码Redis最易被忽视的CPU和内存占用高问题](https://mp.weixin.qq.com/s?__biz=MzI4NTA1MDEwNg==&mid=2650781521&idx=1&sn=c0b0512b636a5e109299171bfa178f5e)
  > - 尽量不要使用短连接；
  > - 尽量不要在连接数比较高的场景下频繁使用info；
  > - 使用pipeline时，要及时接收请求处理结果，且pipeline不宜一次打包太多请求。

* [当 Redis 发生高延迟时，到底发生了什么](https://mp.weixin.qq.com/s?__biz=Mzg2NjE5NDQyOA==&mid=2247483922&idx=1&sn=1dd95a66d654cfd4aee7c31280aef1eb)
* [秒杀系统的艺术](https://juejin.im/post/5d84e21f6fb9a06ac8248149)
* [《吊打面试官》系列-秒杀系统设计](https://juejin.im/post/5dd09f5af265da0be72aacbd)
* [《大厂内部资料》Redis 性能优化的 13 条军规！全网首发](https://mp.weixin.qq.com/s?__biz=MzU1NTkwODE4Mw==&mid=2247484916&idx=1&sn=d49ea56a1725aa140fc222266c1fc32f)
* [Redis 6.0 正式版终于发布了！除了多线程还有什么新功能？](https://mp.weixin.qq.com/s/hMTGgyE6g36DnUoAGDihbw)
  > - 提供了众多的新模块（modules）API
  > - 提供了客户端缓存功能
  > - SSL
  > - ACLs 权限控制
  > - 多线程 I/O 能力
  > - 提升了 RDB 日志的加载速度
* [面试时说Redis是单线程的，被喷惨了！](https://mp.weixin.qq.com/s/o3uw90NFsOAfDAb1zbW5Eg)
  > Redis6 在设计上采用将网络数据读写和协议解析通过多线程的方式来处理，对于命令执行来说，仍然使用单线程操作。
* [硬核！15张图解Redis为什么这么快](https://mp.weixin.qq.com/s/b_yzbLeQh57oYjqlIgPiYQ)
* [缓存与库先写哪个，这十几张图告诉你](https://mp.weixin.qq.com/s/4JcMG9UpAgFqsI1SXaJA2A)
  > 并发量不高：双写一致方案（先删除缓存，后更新数据库）  
  > 高并发首推：缓存延时双删策略方案
* [Redis的bitmap从基础到业务](https://blog.csdn.net/ctwctw/article/details/105013817)
* [SpringBoot2.x中使用Redis的bitmap结构（工具类）](https://www.jianshu.com/p/305e65de1b13)
* [【ProcessOn】Redis—AKF服务拆分原则、CAP理论前置、数据一致性理论与方案](https://www.processon.com/view/5ede3fcc5653bb6963dcb62f)

### 一致性问题
* [Redis缓存和MySQL数据一致性方案详解](https://mikechen.cc/3410.html)
  > - 第一种方案：采用延时双删策略
  > - 第二种方案：异步更新缓存(基于订阅binlog的同步机制)

## 分布式锁
* [面试官：如何用Redis实现分布式锁？](https://juejin.im/post/5e9473f5e51d454702460323)
* [一文看透 Redis 分布式锁进化史（解读 + 缺陷分析）](https://mp.weixin.qq.com/s?__biz=MzUzMTA2NTU2Ng==&mid=2247486492&idx=1&sn=d1bebca555cea270be26bc7db71f2d97)
* [分布式锁-RedisLockRegistry源码分析](https://www.cnblogs.com/f-zhao/p/6836869.html)

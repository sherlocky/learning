# 消息队列
> 常见3大应用场景：异步、削峰（填谷）、解耦。

* [《吊打面试官》系列-消息队列基础](https://juejin.im/post/5dd3ff85e51d453fe34dfcc5)
* [《吊打面试官》系列-分布式事务、重复消费、顺序消费](https://juejin.im/post/5dda9e7e6fb9a07aae2a3778)

## Kafka
> Broker、Topic下 分区(Partition)（一主多备，天然分布式，单分区写入有序）、消费者组、偏移量(offset)（消费者可指定读取）、消息日志等概念。
  消息传递、存储、流处理3大主要功能。
* [全网最通俗易懂的Kafka入门！ - 掘金](https://juejin.im/post/5de706d66fb9a0164f292242)
* [朱小斯--图解 Kafka 之实战指南](https://juejin.im/book/5c7d467e5188251b9156fdc0)
* [朱小斯--图解 Kafka 之核心原理](https://juejin.im/book/5c7d270ff265da2d89634e9e)
* [带你涨姿势的认识一下kafka](https://mp.weixin.qq.com/s?__biz=MzU2NDg0OTgyMA==&mid=2247484570&idx=1&sn=1ad1c96bc7d47b88e976cbd045baf7d7)
* [带你涨姿势是认识一下Kafka Producer](https://mp.weixin.qq.com/s?__biz=MzU2NDg0OTgyMA==&mid=2247484698&idx=1&sn=886292c24485cca9f1f828f3b325fef5)
* [带你涨姿势的认识一下Kafka之消费者](https://mp.weixin.qq.com/s?__biz=MzU3NzczMTAzMg==&mid=2247486105&idx=1&sn=760f131c0a339d1b8e3554870a2b5c0b)
  
* [Kafka 会不会丢消息？怎么处理的?](https://mp.weixin.qq.com/s/tioD1yMABXu8BLj3dGtTmg)
  
## RocketMQ
* [《浅入浅出》-RocketMQ](https://juejin.im/post/5de3c8026fb9a07194761641)

* [RocketMQ 的事务消息](https://halo.sherlocky.com/archives/rocketmq-tx-msg)
* [【官方】RocketMQ事务消息的设计](http://rocketmq.apache.org/rocketmq/the-design-of-transactional-message/)
* [【官方】RocketMQ事务消息使用示例](http://rocketmq.apache.org/docs/transaction-example/)  
* [RocketMQ事务消息学习及刨坑过程](https://blog.51cto.com/14230003/2446308)
* [RocketMq事务消息](https://www.jianshu.com/p/c26b3af5880f)

## RabbitMQ
 * 三种交换机
   > Direct Exchange：  
   > 直连型交换机，根据消息携带的路由键将消息投递给对应队列。  
   > 大致流程，有一个队列绑定到一个直连交换机上，同时赋予一个路由键 routing key 。  
   > 然后当一个消息携带着路由值为X，这个消息通过生产者发送给交换机时，交换机就会根据这个路由值X去寻找绑定值也是X的队列。  
   > Fanout Exchange：  
   > 扇型交换机，这个交换机没有路由键概念，就算你绑了路由键也是无视的。 这个交换机在接收到消息后，会直接转发到绑定到它上面的所有队列。  
   > Topic Exchange：  
   > 主题交换机，这个交换机其实跟直连交换机流程差不多，但是它的特点就是在它的路由键和绑定键之间是有规则的。
 ```bash
 *  (星号) 用来表示一个单词 (必须出现的)
 #  (井号) 用来表示任意数量（零个或多个）单词
 当一个队列的绑定键为 "#"（井号） 的时候，这个队列将会无视消息的路由键，接收所有的消息。
 当 * (星号) 和 # (井号) 这两个特殊字符都未在绑定键中出现的时候，此时主题交换机就拥有的直连交换机的行为。
 所以主题交换机也就实现了扇形交换机的功能，和直连交换机的功能。
 ``` 
 * [Springboot 整合RabbitMq ，用心看完这一篇就够了](https://blog.csdn.net/qq_35387940/article/details/100514134)
 * [RabbitMQ自学之路（五）——-SpringBoot与RabbitMQ整合和对五种队列模式的实现](https://blog.csdn.net/qq_29914837/article/details/93144255)
 * [spring boot 中使用 RabbitMQ 教程三 采用Fanout实现发布与订阅](https://www.jianshu.com/p/8500c285d5c9)
   > AMQP 0-9-1里已经解释，同一队列多个消费者时，已经内置实现了负载均衡的deliver机制，所以一个消息只能被一个消费者消费。
   > 多个消费者如果都想接受消息，只能是不同的队列才能实现。
 * [一个基于RabbitMQ的可复用的事务消息方案](https://www.cnblogs.com/throwable/p/12266806.html)

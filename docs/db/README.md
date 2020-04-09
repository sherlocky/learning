# 数据库
* [MySQL 忘记密码，该怎么办？](https://mp.weixin.qq.com/s?__biz=MzI4NDY5Mjc1Mg==&mid=2247488938&idx=2&sn=919f345ea5dfa6a4b2f5e042c94d4d19)
* [【值得收藏】一份非常完整的Mysql规范](https://www.jianshu.com/p/d7d57b6fb7dd)
* [58同城MySql38条军规](http://mp.weixin.qq.com/s?__biz=MjM5ODYxMDA5OQ==&mid=2651959906&idx=1&sn=2cbdc66cfb5b53cf4327a1e0d18d9b4a)
* [高性能MySQL（第3版）.pdf](https://ghost.oss.sherlocky.com/learning/mysql/%E9%AB%98%E6%80%A7%E8%83%BDMySQL%EF%BC%88%E7%AC%AC3%E7%89%88%EF%BC%89.pdf)
* [面试官问，为什么建议MySQL列属性尽量用 NOT NULL ？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486868&idx=1&sn=b3b17886e89f696c2a0e4aa593329554)
* [项目中常用的19条MySQL优化](https://zhuanlan.zhihu.com/p/49888088)
* [按照这30条建议优化SQL，性能绝对不会太差](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247484182&idx=1&sn=776c152b7bff8df6c176cadfc620d9df)
* [超全面的MySQL语句加锁分析](https://mp.weixin.qq.com/s?__biz=MzIxMjE5MTE1Nw==&mid=2653198050&idx=2&sn=68a6594ac35976532ad6a0eec6dc06dd)
* [年薪50万的DBA必须了解的MySQL锁和事务](https://mp.weixin.qq.com/s?__biz=MzI4NTA1MDEwNg==&mid=2650779014&idx=1&sn=05ceda0ad2c54a4c7d3983692b8c0789)
* [MySQL 是怎样运行的：从根儿上理解 MySQL](https://juejin.im/book/5bffcbc9f265da614b11b731/section/5c238f0851882521eb44c51f)
* [MySQL 8.0+ WITH 语法(Common Table Expressions - CTE)](https://gblog.sherlocky.com/mysql-8-cte/)
* [面试官问：MySQL的自增ID用完了，怎么办？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247487265&idx=1&sn=46029e2d4c630635fd7636141dd90d23)
* [如何基于 MySQL 主从模式搭建上万并发的系统架构？](https://my.oschina.net/u/4205711/blog/3104493)
* [MySQL的COUNT(*)语句](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650124956&idx=1&sn=3bce85cdc1768f71b4332ba8f25278b0)

## 索引
  * [如何理解并正确使用MySql索引](https://my.oschina.net/feinik/blog/1305784)
  * [[慢查优化]建索引时注意字段选择性 & 范围查询注意组合索引的字段顺序](https://my.oschina.net/zhengyun/blog/162985) 
  * [为什么MySQL用B+树做索引](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650125030&idx=1&sn=1c2a09a80547159b336e7ea25d7f4955)

## MySQL 日志
  * [MySQL探秘(四):InnoDB的磁盘文件及落盘机制](https://www.jianshu.com/p/e546ea1fc067)
  * [Mysql Redo Log日志](https://blog.csdn.net/longgeqiaojie304/article/details/98869707)
  * [MySQL Binlog--事务日志和BINLOG落盘参数对磁盘IO的影响](https://www.cnblogs.com/gaogao67/p/11023837.html)
  * [MySQL binlog相关分析](https://www.cnblogs.com/geaozhang/p/7401416.html)
  * [MySQL 的"双1设置"-数据安全的关键参数（案例分享）](https://www.cnblogs.com/kevingrace/p/10441086.html)
  * [mysql的断电恢复能力](https://www.jianshu.com/p/a32762bb11be)

## 分库分表
  * [sharding JDBC --> sharding sphere](https://shardingsphere.apache.org/document/current/cn/quick-start/sharding-jdbc-quick-start/)
  * [不用找了，大厂在用的分库分表方案，都在这了！](https://mp.weixin.qq.com/s?__biz=MzUzMTA2NTU2Ng==&mid=2247487697&idx=1&sn=05c90f0436500d9ea8f68555b07155e3)
  * [数据库分库分表](http://www.cnblogs.com/405845829qq/p/7552736.html)

## MySQL 高可用
  * 小型业务选择M-S 即可；
  * 复杂、重要业务硬件足够选 MHA，其次选PXC；
  * 复杂、重要业务单硬件不足，选M-M，需设立开发、运维规范。
  > MySQL第三方高可用架构：MHA 消耗资源大，健壮性强，前期投入大，后期维护成本小 （日志补偿）  
  可参考：[使用MHA实现MySQL主从复制高可用](https://blog.csdn.net/wzy0623/article/details/81304654)

## MyBatis 
  * [别怕看源码,一张图搞定Mybatis的Mapper原理-肥朝](https://www.jianshu.com/p/419ce7b5c1ce)
    > ![MybatisMapper时序图](https://ghost.oss.sherlocky.com/FoB0EZUy5htr0RZ1Q7yoIfRIJ5Eu-halo)
  * [mybatis思维导图，让mybatis不再难懂（一）](https://my.oschina.net/u/3080373/blog/880501)
  * [mybatis思维导图，让mybatis不再难懂（二）](https://my.oschina.net/u/3080373/blog/884176)
  * [MyBatis 二级缓存详解](https://mp.weixin.qq.com/s/sQLnePy2hMPkCB7xYz3qEQ)
  * [Mybatis面试 18 问](/archives/mybatis)
  * [Mybatis常见面试题总结及答案](https://mp.weixin.qq.com/s/g2VxzeZhJngy4Q-WZCw4EQ)
    > 原地址： [Mybatis常见面试题总结](https://blog.csdn.net/a745233700/article/details/80977133)

## wier 数据库分析系列博文
  * [DB——数据的读取和存储方式](https://my.oschina.net/u/1859679/blog/1581379)
  * [Sql优化器究竟帮你做了哪些工作？](https://my.oschina.net/u/1859679/blog/1586098)
  * [什么是DB的三星索引](https://my.oschina.net/u/1859679/blog/1589575)
  * [如何预估索引性能？](https://my.oschina.net/u/1859679/blog/1592538)
  
## 锁
> 查看死锁：```show engine innodb status;```

 * [Mysql死锁如何排查：insert on duplicate死锁一次排查分析过程](https://juejin.im/post/5d483e66518825052734b15a)
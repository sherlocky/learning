# 数据库
* [MySQL 是怎样运行的：从根儿上理解 MySQL](https://juejin.im/book/5bffcbc9f265da614b11b731/section/5c238f0851882521eb44c51f)
* [MySQL 忘记密码，该怎么办？](https://mp.weixin.qq.com/s?__biz=MzI4NDY5Mjc1Mg==&mid=2247488938&idx=2&sn=919f345ea5dfa6a4b2f5e042c94d4d19)
* [高性能MySQL（第3版）.pdf](https://ghost.oss.sherlocky.com/learning/mysql/%E9%AB%98%E6%80%A7%E8%83%BDMySQL%EF%BC%88%E7%AC%AC3%E7%89%88%EF%BC%89.pdf)
* [年薪50万的DBA必须了解的MySQL锁和事务](https://mp.weixin.qq.com/s?__biz=MzI4NTA1MDEwNg==&mid=2650779014&idx=1&sn=05ceda0ad2c54a4c7d3983692b8c0789)
* [面试官问：MySQL的自增ID用完了，怎么办？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247487265&idx=1&sn=46029e2d4c630635fd7636141dd90d23)
* [如何基于 MySQL 主从模式搭建上万并发的系统架构？](https://my.oschina.net/u/4205711/blog/3104493)
* [MySQL的COUNT(*)语句](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650124956&idx=1&sn=3bce85cdc1768f71b4332ba8f25278b0)
* [MySQL 8.0+ WITH 语法(Common Table Expressions - CTE)](https://gblog.sherlocky.com/mysql-8-cte/)
* [《吊打面试官》系列-数据库基础知识](https://mp.weixin.qq.com/s/NDL1Q6nqdPq5oMBWSpq4ug)
  > MySQL8.0直接把查询缓存的功能删除了。  
  > 不建议使用查询缓存，因为查询缓存往往弊大于利。查询缓存的失效非常频繁，只要有对一个表的更新，这个表上的所有的查询缓存都会被清空。
* [MySQL 的 InnoDB 存储引擎是怎么设计的？](https://mp.weixin.qq.com/s/wr2gJGQSA8QH_lmPh1XOkw)
  > merge：Change Buffer -> Buffer Pool  
  > purge：Buffer Pool -> Disk  
  > Log Buffer  
  > Doublewrite Buffer

* [数据库优化 - 实例优化](https://mp.weixin.qq.com/s?__biz=Mzg3NjE0ODM2NA==&mid=2247483796&idx=1&sn=fe5fbf12670ffd06149b26edc06026fd)
* [为什么不建议把数据库部署在docker容器内？](https://www.toutiao.com/i6805798581971190276)
> 如果容器突然崩溃，数据库未正常关闭，可能会损坏数据。另外，容器里共享数据卷组，对物理机硬件损伤也比较大。
> 即使你要把 Docker 数据放在主机来存储 ，它依然不能保证不丢数据。 Docker volumes 的设计围绕 Union FS 镜像层提供持久存储，但它仍然缺乏保证。

## 连接池
 * [数据库连接池到底应该设多大？这篇文章可能会颠覆你的认知](https://www.jianshu.com/p/a8f653fc0c54)

## 规范
* [【值得收藏】一份非常完整的Mysql规范](https://www.jianshu.com/p/d7d57b6fb7dd)
* [58同城MySql38条军规](http://mp.weixin.qq.com/s?__biz=MjM5ODYxMDA5OQ==&mid=2651959906&idx=1&sn=2cbdc66cfb5b53cf4327a1e0d18d9b4a)
* [面试官问，为什么建议MySQL列属性尽量用 NOT NULL ？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486868&idx=1&sn=b3b17886e89f696c2a0e4aa593329554)

## 优化
* [MySQL 优化实施方案](https://www.cnblogs.com/clsn/p/8214048.html)
* [项目中常用的19条MySQL优化](https://segmentfault.com/a/1190000012155267)
  > 知乎链接，暂无法访问：[项目中常用的19条MySQL优化](https://zhuanlan.zhihu.com/p/49888088)
* [按照这30条建议优化SQL，性能绝对不会太差](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247484182&idx=1&sn=776c152b7bff8df6c176cadfc620d9df)
* MySQL 统计信息
 > 统计信息，默认采样率 20 

## 索引
  * [如何理解并正确使用MySql索引](https://my.oschina.net/feinik/blog/1305784)
  * [[慢查优化]建索引时注意字段选择性 & 范围查询注意组合索引的字段顺序](https://my.oschina.net/zhengyun/blog/162985) 
  * [为什么MySQL用B+树做索引](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650125030&idx=1&sn=1c2a09a80547159b336e7ea25d7f4955)
  * [mysql索引失效的情况](https://www.cnblogs.com/wuchanming/p/8075840.html)

## 锁
  * [超全面的MySQL语句加锁分析](https://mp.weixin.qq.com/s?__biz=MzIxMjE5MTE1Nw==&mid=2653198050&idx=2&sn=68a6594ac35976532ad6a0eec6dc06dd)
  > 锁定读的语句:  
    - SELECT ... LOCK IN SHARE MODE;  
    - SELECT ... FOR UPDATE;  
    - UPDATE ...  
    - DELETE ...  
  > S型正经记录锁、X型正经记录锁  
  > ``索引条件``下推特性只适用于``二级索引``（只是为了减少回表次数，也就是减少读取完整的聚簇索引记录的次数，从而减少IO操作）。  
  > 有时要对``聚簇索引记录``和``二级索引记录``都加锁，顺序要分情况具体分析（由于不同情况加锁顺序可能不同，有可能发生``死锁``）。
  
## MySQL 日志
  * [MySQL binlog、redo log、undo log 简单阐述](https://mp.weixin.qq.com/s/Lx4TNPLQzYaknR7D3gmOmQ)
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
  * [Mybatis源码讲解（三）-- SqlSession](https://mp.weixin.qq.com/s?__biz=MzU3NzczMTAzMg==&mid=2247487402&idx=1&sn=f805e2141f2ef953bdb31218ef75a9ba)
  * [mybatis动态SQL与批量插入](https://juejin.im/post/5e959b355188257382099074)
  
## wier 数据库分析系列博文
  * [DB——数据的读取和存储方式](https://my.oschina.net/u/1859679/blog/1581379)
  * [Sql优化器究竟帮你做了哪些工作？](https://my.oschina.net/u/1859679/blog/1586098)
  * [什么是DB的三星索引](https://my.oschina.net/u/1859679/blog/1589575)
  * [如何预估索引性能？](https://my.oschina.net/u/1859679/blog/1592538)
  
## 死锁
> 查看死锁：```show engine innodb status;```

 * [Mysql死锁如何排查：insert on duplicate死锁一次排查分析过程](https://juejin.im/post/5d483e66518825052734b15a)

## 国产达梦数据库
  * [DM7 达梦数据库安装后配置及调优](//halo.sherlocky.com/archives/dm7-setup-optimize)
  * [记一次对达梦数据库的优化过程](https://hacpai.com/article/1574159839794#慢-SQL-优化)
  * [【干货分享】达梦SQL优化——基础篇](http://www.dameng.com/teachers_view.aspx?TypeId=183&Id=1027)
  * [【干货分享】达梦SQL优化——基础篇(2)](http://www.dameng.com/teachers_view.aspx?TypeId=183&Id=1030)
  * [【干货分享】达梦SQL优化——基础篇(3)](http://www.dameng.com/teachers_view.aspx?TypeId=183&Id=1036)
  * [【干货分享】组合索引中列的顺序问题](https://mp.weixin.qq.com/s?__biz=MzIwNTEyMTgzNw==&mid=2652655003&idx=1&sn=2665f03fa0ed784fcefa82b76a49b528)
  * [【干货分享】DM7倒序排序优化的方法](https://mp.weixin.qq.com/s?__biz=MzIwNTEyMTgzNw==&mid=2652656812&idx=2&sn=fb38d1090d7a2dd42fa9f86fb2e8a13b)
  * [DM7 达梦数据库 查询优化 -- 执行计划 查看](https://www.cndba.cn/cndba/dave/article/3630)
  * [DM7 达梦数据库 快照管理 及 生成 AWR 报告](https://www.cndba.cn/dave/article/3616)
  * [DM7 达梦数据库 索引 管理 说明](https://www.cndba.cn/dave/article/3585)
  
## OLTP VS OLAP
  * OLTP，也叫联机事务处理（Online Transaction Processing）系统
  > 表示事务性非常高的系统，一般都是高可用的在线系统
  * OLAP，也叫联机分析处理（Online Analytical Processing）系统
  > 有的时候也叫DSS决策支持系统，就是我们说的数据仓库。

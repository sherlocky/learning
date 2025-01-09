# 数据库
* 通常我们认为 MySQL 单表数据量达到**5000W**就会有性能瓶颈
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
* [Mysql不锁表增加字段和索引方法](https://c4ys.com/archives/1943)
  > [InnoDB在线DDL操作](https://dev.mysql.com/doc/refman/8.0/en/innodb-online-ddl-operations.html)

* [HAVING的神器用法](https://www.cnblogs.com/youzhibing/p/14175336.html)
  > https://mp.weixin.qq.com/s?__biz=MzAxODcyNjEzNQ==&mid=2247529555&idx=3&sn=d6f33ca56c1824b2c15352f35356a3e5

## MySQL 注释
* 特殊的功能
  > - SQL标准中，多行注释 是 ``/* xxx */``
  > - MySQL扩展了注释功能，``/*! select * from test */``，在起头的``/*``后头加入``!``，那么此注释里的语句将被执行
  > - 另外，/*!50001 select * from test */; 这里的``50001``表示假如 数据库是``5.00.01``以上版本，该语句才会被执行

## MySQL 一致性读
* [阿里面试：说说一致性读实现原理？](https://mp.weixin.qq.com/s/qHzb6oPrrbAPoIlfLJVNAg)
* [敖丙-数据库-微信公众号话题](https://mp.weixin.qq.com/mp/appmsgalbum?__biz=MzAwNDA2OTM1Ng==&action=getalbum&album_id=1343708196397187073&scene=173&from_msgid=2453148068&from_itemidx=1&count=3#wechat_redirect)

## 连接池
 * [数据库连接池到底应该设多大？这篇文章可能会颠覆你的认知](https://www.jianshu.com/p/a8f653fc0c54)

## 规范
* [阿里巴巴MySQL建表规范](https://mp.weixin.qq.com/s/Kif4yvRJGO68jXPErxwNXw)
* [阿里巴巴SQL强制规范，MySQL篇](https://mp.weixin.qq.com/s/h58L7XxIq5MibmGN-GAHCQ)
* [58同城MySql38条军规](http://mp.weixin.qq.com/s?__biz=MjM5ODYxMDA5OQ==&mid=2651959906&idx=1&sn=2cbdc66cfb5b53cf4327a1e0d18d9b4a)
* [面试官问，为什么建议MySQL列属性尽量用 NOT NULL ？](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247486868&idx=1&sn=b3b17886e89f696c2a0e4aa593329554)

## 优化
* [为什么MySQL内存占用这么大？ for InnoDB](https://cloud.tencent.com/developer/article/1536662)
* [mysql使用内存计算器](http://www.mysqlcalculator.com/)
* [MySQL 优化实施方案](https://www.cnblogs.com/clsn/p/8214048.html)
* [项目中常用的19条MySQL优化](https://segmentfault.com/a/1190000012155267)
* [按照这30条建议优化SQL，性能绝对不会太差](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247484182&idx=1&sn=776c152b7bff8df6c176cadfc620d9df)
* MySQL 统计信息
 > 统计信息，默认采样率 20 
* 标量子查询：就是返回单一值的子查询
 > 由于返回的是单一的值，因此标量子查询的返回值可以用在 = 或者 <> 这样需要单一值的比较运算符之中。这也正是标量子查询的优势所在。

## Hash Join
* [MySQL8 的 Hash join 算法](https://zhuanlan.zhihu.com/p/94065716)
  > ![](https://pic1.zhimg.com/v2-e0df14d3667389fb92cd78eae4b2e1f8_r.jpg)

## 索引
  * [如何理解并正确使用MySql索引](https://my.oschina.net/feinik/blog/1305784)
  * [[慢查优化]建索引时注意字段选择性 & 范围查询注意组合索引的字段顺序](https://my.oschina.net/zhengyun/blog/162985) 
  * [为什么MySQL用B+树做索引](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650125030&idx=1&sn=1c2a09a80547159b336e7ea25d7f4955)
  * [mysql索引失效的情况](https://www.cnblogs.com/wuchanming/p/8075840.html)

## 优先队列
* [深入浅出 MySQL 优先队列](https://mp.weixin.qq.com/s/2GoGuG-POHpiqnNb0_Z85A)

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
  * [为什么要把MySQL的binlog格式修改为row](https://cloud.tencent.com/developer/article/1595161)
  * [MySQL binlog、redo log、undo log 简单阐述](https://mp.weixin.qq.com/s/Lx4TNPLQzYaknR7D3gmOmQ)
  * [MySQL探秘(四):InnoDB的磁盘文件及落盘机制](https://www.jianshu.com/p/e546ea1fc067)
  * [Mysql Redo Log日志](https://blog.csdn.net/longgeqiaojie304/article/details/98869707)
  * [MySQL Binlog--事务日志和BINLOG落盘参数对磁盘IO的影响](https://www.cnblogs.com/gaogao67/p/11023837.html)
  * [MySQL binlog相关分析](https://www.cnblogs.com/geaozhang/p/7401416.html)
  * [MySQL 的"双1设置"-数据安全的关键参数（案例分享）](https://www.cnblogs.com/kevingrace/p/10441086.html)
  * [mysql的断电恢复能力](https://www.jianshu.com/p/a32762bb11be)

  * [MySQL不会丢失数据的秘密，就藏在它的 7种日志里](https://mp.weixin.qq.com/s/-v6CHvvAwtuznG-bzZKQ0w)

### MVVC
  * [相见恨晚，MVCC 这么理解，早就通关了](https://mp.weixin.qq.com/s?__biz=MzkwNzI0MzQ2NQ==&mid=2247490423&idx=1&sn=d14308144d96cfca19aaa9582ff0435e&chksm=c0dd61d1f7aae8c721a9096b3cc6a8ff9a3a223dbc3607af236531078c2d22e7b2133a227c7f&scene=21#wechat_redirect)
 
## 分库分表
  * [数据库分库分表](http://www.cnblogs.com/405845829qq/p/7552736.html)
  * [MySQL数据库之互联网常用分库分表方案](https://www.cnblogs.com/littlecharacter/p/9342129.html)
  * [前任都能看懂的分库分表方案](https://mp.weixin.qq.com/s/dMqXBW6W8DeqfAPvko3ViQ)

  * [sharding JDBC --> sharding sphere](https://shardingsphere.apache.org/document/current/cn/quick-start/sharding-jdbc-quick-start/)
  * [芋道 Spring Boot 分库分表入门](http://www.iocoder.cn/Spring-Boot/sharding-datasource/)
    > - Sharding-JDBC 采用无中心化架构，适用于 Java 开发的高性能的轻量级 OLTP 应用。
    > - Sharding-Proxy 提供静态入口以及异构语言的支持，适用于 OLAP 应用以及对分片数据库进行管理和运维的场景。
  
    > Sharding-JDBC ，相比 Sharding-Proxy 来说，是基于 client 模式，无需经过 proxy 一层的性能损耗，也不用考虑 proxy 的高可用，
    > 所以对于 Java 项目来说，更加被推荐。目前，阿里、京东、美团等公司，都采用 client 模式的分库分表中间件。
    > Sharding-JDBC 是 Client 端级别，MyCAT 是 Server 级别。
    > - 京东：采用 client 模式的读写分离和分库分表。
    > - 美团：采用 client 模式的读写分离和分库分表。
    > - 陌陌：采用 client 模式的读写分离和分库分表。
  
  * [**Sharding-JDBC 源码分析**](http://www.iocoder.cn/categories/Sharding-JDBC/?self)
  * [分而治之--浅谈分库分表及实践之路 | 京东云技术团队](https://blog.csdn.net/jdcdev_/article/details/130983844)
  * [一种轻量分表方案](https://mp.weixin.qq.com/s/ZDnQUI7yT9kK9Q5wlU0SZg)

## 读写分离
  * [芋道 Spring Boot 多数据源（读写分离）入门](http://www.iocoder.cn/Spring-Boot/dynamic-datasource/?self)

## MySQL 高可用
  * 小型业务选择M-S 即可；
  * 复杂、重要业务硬件足够选 MHA，其次选PXC；
  * 复杂、重要业务单硬件不足，选M-M，需设立开发、运维规范。
  > MySQL第三方高可用架构：MHA 消耗资源大，健壮性强，前期投入大，后期维护成本小 （日志补偿）  
  可参考：[使用MHA实现MySQL主从复制高可用](https://blog.csdn.net/wzy0623/article/details/81304654)

## ORM 框架

### MyBatis 
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

#### [mybatis使用resultMap解决嵌套属性问题](https://juejin.cn/post/7324253082615463987)
```java
@Data
public class SpuItemAttrGroupVo {
    private String groupName;
    private List<Attr> attrs;
}
@Data
public class Attr {
    private Long attrId;
    private String attrName;   
    private String attrValue;
}
```
```xml
<resultMap id="SpuItemAttrGroupVo" type="com.tomla.gomall.product.vo.SpuItemAttrGroupVo">
    <result property="groupName" column="attr_group_name"></result>
    <collection property="attrs" ofType="com.tomla.gomall.product.vo.Attr">
        <result property="attrId" column="attr_id"></result>
        <result property="attrName" column="attr_name"></result>
        <result property="attrValue" column="attr_value"></result>
    </collection>
</resultMap>
<select id="getSpuItemAttrGroupVo" resultMap="SpuItemAttrGroupVo">
    <!--查询语句略-->
</select>
```

#### MyBatis Plus
  * [【实验】mybatis批量插入方式的比较](https://mp.weixin.qq.com/s/-rfokXqRctRZatwZDmOT3g)
    > 少量插入请使用反复插入单条数据，方便。数量较多请使用批处理方式。
    > （可以考虑以有需求的插入数据量20条左右为界吧，在我的测试和数据库环境下耗时都是百毫秒级的，方便最重要）。  
    > 无论何时都不用xml拼接sql的方式。
  * [MybatisPlus批量插入-mapper层 选装件 InsertBatchSomeColumn](https://gitee.com/baomidou/mybatis-plus/blob/3.0/mybatis-plus-extension/src/main/java/com/baomidou/mybatisplus/extension/injector/methods/InsertBatchSomeColumn.java)
    > 位于``com.baomidou.mybatisplus.extension.injector.methods``包下,需要配合[Sql 注入器](https://baomidou.com/guide/sql-injector.html)使用。
    > 参考：[案例](https://gitee.com/baomidou/mybatis-plus-samples/blob/master/mybatis-plus-sample-sql-injector/src/main/java/com/baomidou/samples/injector/base/MySqlInjector.java)
  * [MybatisPlus真正的批量插入（非循环单个）方法](https://blog.csdn.net/qq_18630487/article/details/111153883)
  * [mybatis-plus真正批量新增和更新](https://www.jianshu.com/p/df14fa887b85)
  * [性能提升 2000%！揭秘 MyBatis-Plus 批量插入的终极优化技巧](https://mp.weixin.qq.com/s/bmqRiv_LwZRgZDfiZInJpA)

### Jooq
现代化的 Java SQL 框架；在性能、效率及开发体验上秒杀 Mybatis

- [官方文档](https://www.jooq.org/doc/3.19/manual-single-page/#Overview)
- [相关教程](https://jooq.diamondfsd.com/learn/section-1-how-to-start.html)
- [jOOQ and Kotlin](https://www.jooq.org/doc/latest/manual/getting-started/jooq-and-kotlin/)

### Jimmer
一个重新思考、重新设计、重新构建的革命性 ORM 框架；颠覆你对整个 JVM 生态的使用体验。

Jimmer的核心理念，在于任意形状的的数据结构作为一个整体进行读写操作，而非简单的处理实体对象。

- [Jimmer官方文档]([Jimmer](https://babyfish-ct.github.io/jimmer-doc/zh/docs/overview/key-features))

## wier 数据库分析系列博文
  * [DB——数据的读取和存储方式](https://my.oschina.net/u/1859679/blog/1581379)
  * [Sql优化器究竟帮你做了哪些工作？](https://my.oschina.net/u/1859679/blog/1586098)
  * [什么是DB的三星索引](https://my.oschina.net/u/1859679/blog/1589575)
  * [如何预估索引性能？](https://my.oschina.net/u/1859679/blog/1592538)
  
## 死锁
> 查看死锁：```show engine innodb status;```

 * [Mysql死锁如何排查：insert on duplicate死锁一次排查分析过程](https://juejin.im/post/5d483e66518825052734b15a)
 * [解决死锁之路（终结篇）- 再见死锁](https://juejin.cn/post/6844903923459817479)
   > [mysql-deadlocks开源项目](https://github.com/aneasystone/mysql-deadlocks)

## 树形结构
  * [左右值编码存储无限分级树形结构设计](https://www.jianshu.com/p/17a8bc823e63) 

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

## ES Elasticsearch
* [全文搜索引擎 ElasticSearch 还是 Solr？](https://www.cnblogs.com/jajian/p/9801154.html)
  > ES 显著功能特点：分布式搜索，多租户，分析搜索，分组和聚合
* [Elasticsearch 技术分析（一）： 基础入门](https://www.cnblogs.com/jajian/p/9976900.html)
* [Elasticsearch 技术分析（二）： 索引映射Mapping问题](https://www.cnblogs.com/jajian/p/10134164.html)
* [Elasticsearch 技术分析（三）： 索引别名Aliases问题](https://www.cnblogs.com/jajian/p/10152681.html)
* [Elasticsearch 技术分析（七）： Elasticsearch 的性能优化](https://www.cnblogs.com/jajian/p/10465519.html)
* [Elasticsearch 技术分析（九）：全文搜索引擎Elasticsearch](https://www.cnblogs.com/jajian/p/11223992.html)
* 自己工作中的一些记录
  > ElasticSearc h索引的``mapping``一旦创建就不能再修改，但可以追加字段定义  
  > ES 的数据写入后其实是不支持修改的，修改的实现为：先标记旧的为删除；复制修改为新的；删除旧的

  > 【es优化】  
  > 磁盘容量 85% 以下，最好独立机器节点，masternode 维护集群状态，不存储数据，配置可以一般，datanode 只存数据配置越高越好，clientnode 负载均衡，cpu 内存要大。  
  > 同一节点禁止分片数据全集。  
  > 索引务必使用别名，每个分片大小不超过30G，分片数不小于节点数，不超过节点数3倍，除非ReIndex，分片数不可变。  
  > 标记为.del的数据会参与检索，定期forcemerge释放空间。  
  > Mapping设置禁止使用默认值，明确数据类型，是否分词，全文检索还是精确匹配。  

  > 路由合计设置，避免大翻页，批量操作bulk接口，禁止SWAP，``swapoff -a``
  > ``segment os cache flush``
  > ``translog os cache flush``

* [基于SpringDataElasticsearch+SpEL表达式实现ES动态索引](https://xeblog.cn/articles/83)
  > 常规写法
  ```java
  @Document(indexName = "xxx-" + "#{ T(xxx.XXXModel).dateStr() }", createIndex = false)
  
  public static String dateStr() {
      return DateUtil.format(new DateTime(), DatePattern.PURE_DATE_FORMAT);
  }
  ```
### ES bulk reject
* [写入拒绝或查询拒绝问题如何解决？
](https://cloud.tencent.com/document/product/845/56274)
  > 解决方案
  > 1. 设置分片大小
  > 分片大小可以通过 index 模板下的 number_of_shards 参数进行配置（模板创建完成后，再次新创建索引时生效，老的索引不能调整）。
  > 2. 调整分片数据不均匀
  > 
* [Elasticsearch分片均衡的情况下，还会出现热写造成的bulk reject？](https://cloud.tencent.com/developer/article/1882973)

### ES 段合并 (segment merge)
* [关于 Elasticsearch 段合并，这一篇说透了！](https://juejin.cn/post/6950104483049242631)
  > 可以减少索引段的数量并提高检索速度；
  > 可以减少索引的容量（文档数） -- 段合并会移除被标记为已删除的那些文档
  >
  > 在速度慢的系统中，段合并会显著影响性能。
* [Elasticsearch 性能调优：段合并(Segment merge) ](https://www.cnblogs.com/8765h/p/14514684.html)

### ``ES`` VS ``Loki``
- [不对全文内容进行索引的Loki到底优秀在哪里，可以占据一部分日志监控领域](https://zhuanlan.zhihu.com/p/371510010)
  > 优点：  
  > 
  > 1.低索引开销  
  >   loki和es最大的不同是 loki只对标签进行索引而不对内容索引，这样做可以大幅降低索引资源开销(es无论你查不查，巨大的索引开销必须时刻承担)  
  > 2.并发查询+使用cache  
  >   同时为了弥补没有全文索引带来的查询降速使用，Loki将把查询分解成较小的分片，可以理解为并发的grep  
  > 3.和prometheus采用相同的标签，对接alertmanager  
  >   Loki和Prometheus之间的标签一致是Loki的超级能力之一  
  > 4.使用grafana作为前端  

- [ELK、Loki日志方案比较](https://www.ctyun.cn/developer/article/418138645577797)

## NoSQL
* [LSM树详解](https://zhuanlan.zhihu.com/p/181498475)

## 实时数据同步 CDC
* CDC 的全称是``Change Data Capture``，在广义的概念上，只要是能捕获数据变更的技术，我们都可以称之为 CDC。
* [Flink CDC 2.0 正式发布，详解核心改进](https://developer.aliyun.com/article/786600)

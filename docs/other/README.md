# 其他
* [free-programming-books](https://github.com/EbookFoundation/free-programming-books/blob/master/free-programming-books-zh.md)
* [干货收藏 | Java程序员必备的一些流程图](https://mp.weixin.qq.com/s/oTE_hbJtI_n6XTx9jj8w9A)
* [牛人自制“神器”，2017 最新 Web 开发者成长路线图](https://www.oschina.net/news/82966/web-developer-roadmap-in-2017?winzoom=1)

## 文件上传

### 分片上传
* [Tus协议 断点续传](https://tus.io/)
  > - [基于Tus协议的文件上传流程](https://food-billboard.github.io/2020/12/28/%E5%9F%BA%E4%BA%8ETus%E5%8D%8F%E8%AE%AE%E7%9A%84%E6%96%87%E4%BB%B6%E4%B8%8A%E4%BC%A0%E6%B5%81%E7%A8%8B/)
  > - [Tus Java 客户端](https://github.com/tus/tus-java-client)

## 命名
* [命名备忘录](https://mp.weixin.qq.com/s/yOgv9H3qc3Ok2Ga2PSi21g)
  > [naming-cheatsheet](https://github.com/kettanaito/naming-cheatsheet)

## 角色权限
* [手把手教你搞定菜单权限设计，精确到按钮级别](https://mp.weixin.qq.com/s?__biz=MzU3NzczMTAzMg==&mid=2247488983&idx=1&sn=c4e38710cbb200fe4944f69ea5de8372)
* [RBAC权限管理（基于角色的访问控制方法）](https://my.oschina.net/zjllovecode/blog/1601002)
* [SpringBoot-RBAC用户角色权限](https://springboot.plus/guide/rbac.html)

## 规则引擎
* [规则引擎框架liteflow](https://liteflow.cc/pages/5816c5/)
* [OptaPlanner 基本概念 - 规划问题， 约束，方案](https://cloud.tencent.com/developer/article/1500049)
* [动态规划-背包问题(01背包、完全背包、多重背包)](https://cloud.tencent.com/developer/article/1697983)

## 搜索引擎
* [倒排索引/全文搜索基本原理](https://www.cnblogs.com/gered/p/9561710.html)

## 消息推送
* [科普一下消息推送Push是怎么做的](https://mp.weixin.qq.com/s/WT4U16vlC15lEx88Ll6OxA)

## 技术
* [先来半打分布式调度系统/框架](https://my.oschina.net/gitosc/blog/894187)
* [一些优秀的网络爬虫工具](https://my.oschina.net/gitosc/blog/880554)
* [YAML](http://www.ruanyifeng.com/blog/2016/07/yaml.html?f=tt)
* [浅谈微服务之API网关](https://cloud.tencent.com/developer/news/257354)
* [微服务部署：蓝绿部署、滚动部署、灰度发布、金丝雀发布](https://www.jianshu.com/p/022685baba7d)
* [浅析VO、DTO、DO、PO的概念、区别和用处（POJO）](https://www.cnblogs.com/qixuejia/p/4390086.html)
* [如何设计一个安全的对外接口](https://my.oschina.net/OutOfMemory/blog/3131916)

## 磨刀不误砍柴工
* [Code Review最佳实践](https://www.cnblogs.com/dotey/p/11216430.html)

## 支付
* [Spring MVC+Spring+MyBatis实现支付宝扫码支付功能（图文详解）](https://mp.weixin.qq.com/s?__biz=MzU0MzQ5MDA0Mw==&mid=2247488039&idx=1&sn=9bb5ba8db210fabf0871e9997152984d)
* [【纯干货】浅析微信支付](https://yclimb.gitbook.io/wxpay)
* [【干货】一文搞懂“订单、账单、支付单”关系](https://mp.weixin.qq.com/s/LwfnSxsF-yQ5fDez-AA9Yw)
  > ![image](https://github.com/user-attachments/assets/cfd49831-bd9d-416a-bb5b-a75b4fd90896)
  > 在交易核心有3个单据，分别是**订单、账单、账单支付记录**，他们之间是一对多对多的关系.
  > 券系统核销了该券：核销记录与账单支付记录之间建立了关联.
  > 一笔支付可能会请求渠道多次，因此我们还会建立一个支付请求的明细，支付单和支付请求之间是1对多的关系。
  > 
  > 在支付核心会产生2类单据： 
  > - 一类是正向支付的支付单和支付请求明细； 
  > - 第二类是退款单和退款请求明细
  >
  > 逆向订单退款就容易多了，因为逆向是正向的反方向，所以涉及到的依然是3个核心，依然是上述的单据维度，只不过单据变成了逆向单，
  > 即**订单变成了退单，账单变成了退款账单、账单支付记录变成了账单退款记录、支付单变成了退款单**等。
* 大支付系统
  > 整个大支付体系可以抽象成12个字：**买、收、付、退、充、提、转、调、算、结、管、对**
  > 
  > 买：交易体系的能力，支付的业务起源；
  > 收付退：支付核心的主要支付能力；
  > 充提转：钱包的支付能力；
  > 调：资金管理系统的支付能力；
  > 算结管：是清结算的处理能力；
  > 对：就是对账，确保数据的一致性

## Android
* [你逃不掉的APK安装原理](https://www.jianshu.com/p/d2a550a953e0)

## 机器学习
* [机器学习必备手册](https://yq.aliyun.com/articles/221644?utm_content=m_33150)
* [适合入门的8个趣味机器学习项目](https://yq.aliyun.com/articles/221708?utm_content=m_33352)
* [漫画：什么是中台？](https://mp.weixin.qq.com/s?__biz=MzIxMjE5MTE1Nw==&mid=2653199744&idx=1&sn=dceaa1a3b68277471985489fb9afebba)
  > 业务中台、技术中台、数据中台、算法中台  
  项目 0 -> 1 无需中台  
  项目 1 -> N 适合中台  
  项目 N -> N + 1 势在必行
  
## 火焰图
* [如何读懂火焰图？](http://www.ruanyifeng.com/blog/2017/09/flame-graph.html)

## 日程
- https://icalendar.org/iCalendar-RFC-5545/3-8-5-3-recurrence-rule.html
- https://tools.ietf.org/html/rfc2445#section-4.3.10
- [日历设计之重复事件规则设计](https://www.cnblogs.com/jcli/p/calendar_recur_rule.html)
  > https://github.com/hongfuli/simplecal

## 视频转码
- [HLS、m3u8、ts]https://juejin.cn/post/6954761121727250439)

## WiFi
- [WiFi 6E](https://info.support.huawei.com/info-finder/encyclopedia/zh/WiFi+6E.html)
  > ![](https://ghost.oss.sherlocky.com/halo/wifi6e.png)
- [WiFi 7]
  > ![](https://ghost.oss.sherlocky.com/halo/wifi7.png)

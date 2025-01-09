# Spring
  * [Spring的BeanUtils的copyProperties方法需要注意的点](https://www.jianshu.com/p/357b55852efc)
  * [Spring 常见面试问题](https://juejin.im/post/5cbda379f265da03ae74c282)
  * [Spring思维导图，让spring不再难懂（一）](https://my.oschina.net/u/3080373/blog/891918)
  * [Spring思维导图，让Spring不再难懂（ioc篇）](https://my.oschina.net/u/3080373/blog/903341)
  * [Spring中获取request的几种方法，及其线程安全性分析](https://www.cnblogs.com/kismetv/p/8757260.html)
  * [我这样回答了Spring 5的新特性，面试官对我刮目相看](https://mp.weixin.qq.com/s/Mt3w49YhNU8plvzuGYuTPQ)
  * [Spring中的循环依赖](https://mp.weixin.qq.com/s/wykX4CdrHT1tvSz2-24NEQ)
    > 
    |依赖情况	|依赖注入方式	|循环依赖是否被解决|
    |:-------|:----|:----|
    |AB相互依赖（循环依赖）	|均采用setter方法注入	|是|
    |AB相互依赖（循环依赖）	|均采用构造器注入	|否|
    |AB相互依赖（循环依赖）	|A中注入B的方式为setter方法，B中注入A的方式为构造器	|是|
    |AB相互依赖（循环依赖）	|B中注入A的方式为setter方法，A中注入B的方式为构造器	|否|
    
    > 面试官：”Spring是如何解决的循环依赖？“
    答：Spring通过三级缓存解决了循环依赖，其中一级缓存为单例池（singletonObjects）,二级缓存为早期曝光对象earlySingletonObjects，三级缓存为早期曝光对象工厂（singletonFactories）。当A、B两个类发生循环引用时，在A完成实例化后，就使用实例化后的对象去创建一个对象工厂，并添加到三级缓存中，如果A被AOP代理，那么通过这个工厂获取到的就是A代理后的对象，如果A没有被AOP代理，那么这个工厂获取到的就是A实例化的对象。当A进行属性注入时，会去创建B，同时B又依赖了A，所以创建B的同时又会去调用getBean(a)来获取需要的依赖，此时的getBean(a)会从缓存中获取，第一步，先获取到三级缓存中的工厂；第二步，调用对象工工厂的getObject方法来获取到对应的对象，得到这个对象后将其注入到B中。紧接着B会走完它的生命周期流程，包括初始化、后置处理器等。当B创建完后，会将B再注入到A中，此时A再完成它的整个生命周期。至此，循环依赖结束！
    
    > 面试官：”为什么要使用三级缓存呢？二级缓存能解决循环依赖吗？“
    答：如果要使用二级缓存解决循环依赖，意味着所有Bean在实例化后就要完成AOP代理，这样违背了Spring设计的原则，Spring在设计之初就是通过``AnnotationAwareAspectJAutoProxyCreator``这个后置处理器来在Bean生命周期的最后一步来完成AOP代理，而不是在实例化后就立马进行AOP代理。

## Spring AOP
  * [6种 @Transactional 注解失效场景](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247483977&idx=1&sn=7d8d3c89bfe2261f6422572dca405990)
  *  @Transactional 失效总结
    > - @Transactional 加于private方法, 无效
    > - @Transactional 加于未加入接口的public方法, 再通过普通接口方法调用, 无效
    > - @Transactional 加于接口方法, 无论下面调用的是private或public方法, 都【有效】
    > - @Transactional 加于接口方法后, 被本类普通接口方法直接调用, 无效
    > - @Transactional 加于接口方法后, 被本类普通接口方法通过接口调用, 【有效】
    > - @Transactional 加于接口方法后, 被它类的接口方法调用, 【有效】
    > - @Transactional 加于接口方法后, 被它类的私有方法调用后, 【有效】
  * [Spring AOP 不生效的坑](https://mp.weixin.qq.com/s/Q0Q3ropapmMRE_mQE68b8Q)
  * [spring中expose-proxy的作用与原理](https://www.cnblogs.com/mzcx/p/11430846.html)

## Spring 5
  * [一文带你了解 Spring 5.0 WebFlux 应用场景 （异步非阻塞式的 Web 框架）](https://www.cnblogs.com/quanxiaoha/p/10773773.html)
    - Spring MVC 因为是使用的同步阻塞式，更方便开发人员编写功能代码，Debug 测试等，一般来说，如果 Spring MVC 能够满足的场景，就尽量不要用 WebFlux;
    - WebFlux 默认情况下使用 ``Netty`` 作为服务器;
    - WebFlux 不支持 MySql，可以支持MongoDB;
    - 特别适合应用在 IO 密集型的服务中（比如微服务网关）
    - 并不能使接口的响应时间缩短，它仅仅能够提升吞吐量和伸缩性
     （IO线程和工作线程分离，单请求处理时长改变不了，但通过提高吞吐量，单位时间处理的请求增多了）
    > 在 WebFlux 中，``Mono``、``Flux``是非阻塞的写法，只有这样，你才能发挥 WebFlux 非阻塞 + 异步的特性。
    > 这哥俩均能充当响应式编程中发布者的角色，不同的是：
    > - Mono：返回 0 或 1 个元素，即单个对象。
    > - Flux：返回 N 个元素，即 List 列表对象。

### Spring 5 源码分析
  * [【PDF】Spring源码分析(第二版)_第二章](https://ghost.oss.sherlocky.com/learning/spring/%E5%92%95%E6%B3%A1%E5%AD%A6%E9%99%A2_Spring%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%28%E7%AC%AC%E4%BA%8C%E7%89%88%29_%E7%AC%AC%E4%BA%8C%E7%AB%A0.pdf)
  * [【PDF】Spring源码分析(第二版)_第三章](https://ghost.oss.sherlocky.com/learning/spring/%E5%92%95%E6%B3%A1%E5%AD%A6%E9%99%A2_Spring%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%28%E7%AC%AC%E4%BA%8C%E7%89%88%29_%E7%AC%AC%E4%B8%89%E7%AB%A0.pdf)
  * [【PDF】Spring源码分析(第二版)_第四章](https://ghost.oss.sherlocky.com/learning/spring/%E5%92%95%E6%B3%A1%E5%AD%A6%E9%99%A2_Spring%E6%BA%90%E7%A0%81%E5%88%86%E6%9E%90%28%E7%AC%AC%E4%BA%8C%E7%89%88%29_%E7%AC%AC%E5%9B%9B%E7%AB%A0.pdf) 

## SpringBoot
  * [自己的Springboot相关博客](//halo.sherlocky.com/archives/springboot)
  * [【Gitee】自己的SpringBoot学习记录](https://gitee.com/sherlocky/springboot2-learning)
  * [spring-boot-plus](https://springboot.plus/guide/)
  * [使用Spring Cache集成Redis](https://blog.battcn.com/2018/05/13/springboot/v2-cache-redis/)
  * [使用 Keycloak 轻松保护 Spring Boot 应用程序](https://www.oschina.net/translate/easily-secure-your-spring-boot-applications-with-k)
  * [优化你的Spring Boot](https://mp.weixin.qq.com/s?__biz=MzI4ODQ3NjE2OA==&mid=2247485244&idx=1&sn=1e5a29a5b3d31b15d93eed538a2530de)
  * [每天用SpringBoot，还不懂RESTful API返回统一数据格式是怎么实现的？](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483905&idx=1&sn=99d294f0ee5127e827a879a8c96ec08d)
  * [新手也能看懂的 SpringBoot 异步编程指南](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650124909&idx=2&sn=74cf031b6e093df554bccf6ddca191f5)
  * [一起来学SpringBoot -- 唐亚峰](https://blog.battcn.com/categories/SpringBoot/)
  * [纯洁的微笑 - SpringBoot 系列文章](http://www.ityouknow.com/spring-boot.html)
  * [Springboot 优雅停止服务的几种方法](https://www.cnblogs.com/huangqingshi/p/11370291.html)
  * [Spring Boot **2.3.0** 如何优雅停机](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247490012&idx=1&sn=26ad26f9d90ccfafea012d61621326b1)
  * [Springboot实现全局日期格式化](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247484028&idx=1&sn=651c8de95979f42a10270e46275c8346)
  * [SpringBoot+Mybatis配置多数据源及事务方案](https://juejin.im/post/5eba38aa6fb9a043777c9b3a)
  * [spring-boot项目最优雅的http客户端工具: Retrofit](https://juejin.im/post/6854573211426750472)
    > [Retrofit官方文档地址](https://square.github.io/retrofit/)，可代替 RestTemplate 或者 okhttp
  * [【精品】Springboot启动扩展点超详细总结](https://www.jianshu.com/p/38d834db7413)
  * [如何控制springboot中bean的加载顺序](https://www.jianshu.com/p/cbcd963fca36)
  * [SpringBoot入门之事件监听](https://www.cnblogs.com/senlinyang/p/8496099.html)
  
### Resource 
  * [SpringBoot读取Resource下文件的几种方式](https://www.jianshu.com/p/7d7e5e4e8ae3)

### 常用内置方法
  * [请不要自己写，Spring Boot非常实用的内置功能](https://mp.weixin.qq.com/s/9e1R9eVWNgy9M2qLENBg5Q)

### Spring Shiro
  * [并发登录人数控制——《跟我学Shiro》](https://www.iteye.com/blog/jinnianshilongnian-2039760)
  * [Shiro+JWT权限管理](https://springboot.plus/guide/shiro-jwt.html#shiro)
  
### Spring Boot Admin
  * [使用 spring-boot-admin 对 Spring Boot 服务进行监控](http://www.ityouknow.com/springboot/2018/02/11/spring-boot-admin.html)
  * [spring-boot-admin](https://github.com/codecentric/spring-boot-admin)

### SpringBoot 脚手架
- [RuoYi](https://doc.ruoyi.vip/ruoyi/)
- [JeecgBoot](https://github.com/jeecgboot/jeecgboot)
  > 4w+星，企业级低代码平台

## SpringCloud
  * [面试官：兄弟，说说 Spring Cloud 的核心架构原理吧](https://mp.weixin.qq.com/s?__biz=MzI4NDY5Mjc1Mg==&mid=2247489127&idx=2&sn=5cba4e2c5e38e7706691014ec9379665)
  * [一起来学SpringCloud -- 唐亚峰](https://blog.battcn.com/categories/SpringCloud/)
  * [纯洁的微笑 - SpringCloud 系列文章](http://www.ityouknow.com/spring-cloud.html)
  * [【程序员DD】Spring Cloud 从入门到精通](http://blog.didispace.com/spring-cloud-learning/)
  * [外行人都能看懂的SpringCloud](https://mp.weixin.qq.com/s?__biz=MzAwNDA2OTM1Ng==&mid=2453140943&idx=1&sn=72ef2d1aa0a5a0265babfdce7234cefd)
  * [实战 Spring Cloud 微服务架构下的“秒杀”（含代码）](https://mp.weixin.qq.com/s?__biz=MzI4ODQ3NjE2OA==&mid=2247485875&idx=1&sn=0ff0a0c4ea9c5a36334d80de83f1084c)
    > 代码：https://github.com/coderliguoqing/distributed-seckill/
  * [Spring Cloud中国社区](http://springcloud.cn)
  
### 优秀项目推荐
  * [【GVP】jeecp/open-capacity-platform](https://gitee.com/owenwangwen/open-capacity-platform)
    > [【看云】配套文档](https://www.kancloud.cn/owenwangwen/open-capacity-platform/1048256)
  
## Spring Cloud Alibaba
  * [alibaba/Sentinel](https://github.com/alibaba/Sentinel/wiki/%E4%BB%8B%E7%BB%8D)
  * [alibaba/Spring Cloud Alibaba Sentinel](https://github.com/alibaba/spring-cloud-alibaba/wiki/Sentinel)
  * [Spring Cloud Alibaba基础教程：使用Sentinel实现接口限流](http://blog.didispace.com/spring-cloud-alibaba-sentinel-1/)
  * [Spring Cloud Alibaba基础教程：@SentinelResource注解使用详解](http://blog.didispace.com/spring-cloud-alibaba-sentinel-2-5/)

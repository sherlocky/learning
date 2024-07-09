# Java
* [【博客】Java知识杂记](https://halo.sherlocky.com/archives/java)
* [🌟**Java个体户**](https://www.javaself.cn/)
* [Java后端线上问题排查常用命令收藏](https://mp.weixin.qq.com/s?__biz=MzAxODcyNjEzNQ==&mid=2247529555&idx=2&sn=6ed56b565cc1af151cb7c3d88fffe422)
* [高效Effective Java第3版-中文在线](https://sjsdfg.github.io/effective-java-3rd-chinese/#/)
* [细思极恐-你真的会写java吗](http://lrwinx.github.io/2017/03/04/%E7%BB%86%E6%80%9D%E6%9E%81%E6%81%90-%E4%BD%A0%E7%9C%9F%E7%9A%84%E4%BC%9A%E5%86%99java%E5%90%97/)
* [如何优雅的将DTO转化成BO](https://blog.csdn.net/lw7551/article/details/62426579)
* [Java 编程技巧之数据结构](https://mp.weixin.qq.com/s?__biz=MzIxNjA5MTM2MA==&mid=2652436181&idx=1&sn=c663d709965f652a91b3baba208f2aa3)
* [正确的打日志姿势](http://lrwinx.github.io/2018/01/25/正确的打日志姿势/)
* [撸个注解（Annotation）有什么难的](https://mp.weixin.qq.com/s?__biz=MzU1NTkwODE4Mw==&mid=2247485045&idx=2&sn=447ab489635289ef5bb089efb7f1830e)
* [Java避坑之解决重复提交的bug](https://mp.weixin.qq.com/s?__biz=MzAxNTM4NzAyNg==&mid=2247483997&idx=1&sn=8bea08bfa81e97d487a5992b47293674)
* [Java代码性能优化的 40+ 细节](https://mp.weixin.qq.com/s/xRfn558-FzPc_edJU6eJYA)
* [50 个 Java 开发常见错误及规避技巧 （Part 1）](https://www.oschina.net/translate/50-common-java-errors-and-how-to-avoid-them-part-1)
* [50 个 Java 开发常见错误及规避技巧 （Part 2）](https://www.oschina.net/translate/50-common-java-errors-and-how-to-avoid-them-part-2)
* [ StackTraceElement获取方法调用栈的信息](http://blog.csdn.net/hp910315/article/details/52702199)
* [Google Guava教程](http://www.yiibai.com/guava/)
* [神奇的Java僵尸(defunct)进程问题排查过程](https://www.jianshu.com/p/f0baed94128e)

* [Object o = new Object() 在内存中占了多少字节](https://blog.csdn.net/u011727756/article/details/106546178/)
> ![锁的升级过程_32位](https://ghost.oss.sherlocky.com/halo/锁的升级过程_32位_1591704088277.png-halo)
> ![锁的升级过程_64位](https://ghost.oss.sherlocky.com/halo/锁的升级过程_64位_1591704088280.png-halo)

## JDK 下载
* 各种JAVA JDK的镜像分发：[injdk](https://www.injdk.cn/)
* [O记JDK下载](https://www.oracle.com/java/technologies/javase-downloads.html)
  > 华为镜像：https://repo.huaweicloud.com/java/jdk/
  > 鉴于JDK偶数版和奇数版的区别(可参考：[JDK 版本号区别](//halo.sherlocky.com/archives/java#jdk-%E7%89%88%E6%9C%AC%E5%8F%B7%E5%8C%BA%E5%88%AB))，如果使用O记JDK8，应该选择8u251
  >
  > 历史版本存档：
  > - [Java SE 8 Archive Downloads (JDK 8u202 and earlier)](https://www.oracle.com/java/technologies/javase/javase8-archive-downloads.html)
  > - [Java SE 8 Archive Downloads (JDK 8u211 and later)](https://www.oracle.com/java/technologies/javase/javase8u211-later-archive-downloads.html)
* [新时代JDK版本的选择](https://mp.weixin.qq.com/s?__biz=MzIzODYyNjkzNw==&mid=2247484056&idx=1&sn=a81a69f123d519014d03ec22c3c3cca4)
* [我应该使用哪个版本的 JDK？](https://juejin.cn/post/7205162789156732986)
* [AdoptOpenJDK下载](https://adoptopenjdk.net/)
  > 清华镜像地址 https://mirrors.tuna.tsinghua.edu.cn/Adoptium/8/jdk/
* 【国产化】JDK选择
  - 华为 毕昇JDK
    > https://www.hikunpeng.com/developer/devkit/download/jdk
    > 只有Linux版
  - [阿里龙井 Alibaba Dragonwell OpenJDK](https://github.com/dragonwell-project/dragonwell8)
    > 提供 Java 8 和 Java 11 两个版本，支持 x64 和 arm 架构。  
    > [Alibaba Dragonwell 下载镜像地址](https://github.com/dragonwell-project/dragonwell8/wiki/%E4%B8%8B%E8%BD%BD%E9%95%9C%E5%83%8F(Mirrors-for-download))
    > 
    > 主要有两个版本：标准版(Standard Edition)和扩展版(Extended Edition)。
    > 
    > **标准版(Standard Edition)**：基于OpenJDK，包含了许多增强功能，包括bug修复，安全补丁，工具支持等。它完全遵循Java SE标准，主要用于一般的使用场景。
    > 
    > **扩展版(Extended Edition)**：在标准版的基础上增加了大量定制特性，主要面向云计算环境进行优化。这些特性已在阿里巴巴的生产环境中得到大规模验证。例如，它包括了诸多特色功能，如JWarmup等。此版本适用于需要使用这些特性，或在阿里云环境中进行Java开发的场景。
    > 
    > 选择哪个版本主要取决于你的具体需求，如果你需要在云环境中进行Java开发，或需要使用阿里巴巴定制的特性，那么扩展版可能更适合你。反之，如果你的需求相对普通，那么标准版可能更能满足你的要求。
* [IBM eclipse openj9](https://github.com/eclipse-openj9/openj9)
  > 基于OpenJDK进行改造，OpenJ9的特点就是性能：低内存占用，快速启动，高吞吐。
  > 通过将 HotSpot 更换为 OpenJ9，内存占用能降低至少 60%，而启动时间也能快 40% 以上，效果立竿见影。
  > 容器场景下更能发挥 OpenJ9 的作用。

  - [ibm-semeru-runtimes](https://developer.ibm.com/languages/java/semeru-runtimes/downloads)
    >  openj9是以前ibm不要的项目，搞砸了，丢给eclipse去搞。 
    > 现在慢慢改好了，改好了之后就拿回去，自己搞了，继续做成ibm版本的java。
    > Docker镜像地址：[ibm-semeru-runtimes](https://hub.docker.com/_/ibm-semeru-runtimes)

  - [有了HotSpot JVM为什么还需要OpenJ9？](https://segmentfault.com/a/1190000043384478)

  - openj9 jvm 参数
    > jvm参数有一些区别，比如：没有参数：``-XX:MetaspaceSize``
    > 
    > 具体可参考 https://www.eclipse.org/openj9/docs/xx_jvm_commands/
    > 
    > https://www.eclipse.org/openj9/docs/xenableexplicitgc/

    - 内存 dump命令为：``jcmd 8 Dump.heap /root/heap-dump.phd``  （8为进程号）
    - 禁止system.gc() ``-XX:-DisableExplicitGC``  
  - dump分析
    > 须使用IBM Semeru Runtimes Java 17 JDK + （支持DTFJ） 的MAT才能打开 
    > https://www.ibm.com/support/pages/eclipse-memory-analyzer-tool-dtfj-and-ibm-extensions



## J2SE
  * [Java 编程思想（中文版）在线](https://lingcoder.github.io/OnJava8/#/sidebar)
  * [Comparison method violates its general contract](https://github.com/y836097668/interview/blob/master/javase/src/main/java/com/sherlocky/interview/javase/compare/ComparatorTest.java)
  > JDk7 下使用 Collections.sort 手动实现的 Comparator 报错 Comparison method violates its general contract
  * [Timsort详解](https://www.jianshu.com/p/892ebd063ad9)
  * [String hashCode 方法为什么选择数字31作为乘子](http://www.tianxiaobo.com/2018/01/18/String-hashCode-方法为什么选择数字31作为乘子/)
  * [StringJoiner](https://www.jianshu.com/p/469fe8fdd3be)

  * [[译]Java中9个处理Exception的最佳实践](https://www.rowkey.me/blog/2017/09/17/java-exception/)
  * [国外大佬给出的三种处理异常的套路！](https://mp.weixin.qq.com/s/XTiFc2DwAVWE3CYa2Im1qw)
  > 有三种处理异常的基本模式：转换（translate）、重试（retry）和恢复（recover）。
  * [注意System.currentTimeMillis()潜在的性能问题](https://www.jianshu.com/p/d2039190b1cb)
  * [System.currentTimeMillis的性能真有如此不堪吗？](https://juejin.im/post/6887743425437925383)
  * [Java Switch 是如何支持 String 的，为什么不支持 long](https://mp.weixin.qq.com/s/dhxXeYR2Sn28Sq_W93aMsw)

## I/O
  * [压缩20M文件从30秒到1秒的优化过程](https://www.jianshu.com/p/25b328753017)

## JDK 7
 * [深入理解 Java try-with-resource 语法糖](https://juejin.im/entry/57f73e81bf22ec00647dacd0)

## JDK 8
  * [Java8 Lambda表达式详解手册及实例](https://mp.weixin.qq.com/s?__biz=MzkwNzI0MzQ2NQ==&mid=2247488946&idx=2&sn=5f92781283af622397984fab54ffd5fd)
  * [Lambda VS 内部类](https://github.com/CarpenterLee/JavaLambdaInternals/blob/master/2-Lambda%20and%20Anonymous%20Classes(II).md)
  * [使用Stream API优化代码](https://juejin.im/post/5d8226d4e51d453c135c5b9a)
  * [Java8 中用法优雅的 Stream，性能也"优雅"吗？](https://mp.weixin.qq.com/s?__biz=MzU0MzQ5MDA0Mw==&mid=2247486142&idx=2&sn=2d9aa6b43a0314d35377a125ac2f13d7)
  * [聊聊 Java8 以后各个版本的新特性](https://juejin.im/post/5d5950806fb9a06b0a277412#heading-47)
  * [别用 Date 了，来试试 LocalDate、LocalTime、LocalDateTime](https://mp.weixin.qq.com/s?__biz=MzU1NTkwODE4Mw==&mid=2247484960&idx=2&sn=b8142c4ffd9fde8e38702890708047ca)
  
  * [Java8 Stream：2万字20个实例，玩转集合的筛选、归约、分组、聚合](https://blog.csdn.net/mu_wind/article/details/109516995)
  * [Java 8 compute ，让 Map 操作更轻松](https://zhuanlan.zhihu.com/p/357230000)
  
## JDK 8 +
  * [JDK8+ 新特性](https://halo.sherlocky.com/archives/jdk8plus)

  * [Java 9的模块化--壮士断"腕"的涅槃](https://zhuanlan.zhihu.com/p/24800180)
  * [Java 11 已发布，String 还能这样玩！](https://mp.weixin.qq.com/s?__biz=MzI3ODcxMzQzMw==&mid=2247487905&idx=1&sn=03887852dc635539f15fd5fc9fd5b88e&scene=21#wechat_redirect)
  * [Java 11 正式发布，这 8 个逆天新特性教你写出更牛逼的代码](https://mp.weixin.qq.com/s?__biz=MzI3ODcxMzQzMw==&mid=2247487206&idx=1&sn=a8ccb604f8508bf296dbd7b25d8fb80f&scene=21#wechat_redirect)
  * [Java 12 骚操作， String居然还能这样玩！](https://mp.weixin.qq.com/s?__biz=MzI3ODcxMzQzMw==&mid=2247490433&idx=2&sn=0b35f6166c7a073eb3e8f05d58ca38db&scene=21#wechat_redirect)
  * [Java 14 之模式匹配，非常赞的一个新特性！](https://mp.weixin.qq.com/s?__biz=MzI3ODcxMzQzMw==&mid=2247493274&idx=1&sn=9aa8abcd70ce58d7ee6c0a44d73c8cf1&scene=21#wechat_redirect)
  * [Java 15 正式发布， 14 个新特性，刷新你的认知！！](https://mp.weixin.qq.com/s?__biz=MzI3ODcxMzQzMw==&mid=2247507309&idx=1&sn=e78cfee56a2b5cd617c0370f64f4c83d&scene=21#wechat_redirect)
  * [JDK 16 正式发布，一次性发布 17 个新特性](https://mp.weixin.qq.com/s/NBjbZuO1E_BJWjmim8C_Vw)
  * [JDK 17 发布，Oracle 宣布从 JDK 17 开始正式免费](https://mp.weixin.qq.com/s/O8eHiLctnMB2UfokcoPrZQ)
    > Java 17+ 可以免费使用了，包括商用
    > JDK 17 是自 2018 年 JDK 11 后的第二个长期支持版本，支持到 2029 年 9 月
    > 第三个长期支持版本是 JDK 21，时间为 2023 年 9 月（LTS 改成了 2 年一次，非 LTS 还是半年一次，下一次计划在 2022/03 发布）
  * [4.6 W 字总结！Java 11—Java 17特性详解](https://mp.weixin.qq.com/s/cIezaR_cqDi9WxxQNCCrBw)
  * [Java 17 升级指南（持续更新）](https://juejin.cn/post/7117531586232320031)
  * 下载地址
    > https://download.oracle.com/java/17/latest/jdk-17_windows-x64_bin.zip  
    > https://download.oracle.com/java/17/latest/jdk-17_linux-x64_bin.tar.gz  
    > OpenJDK 17 发布地址：  
    > http://openjdk.java.net/projects/jdk/17/  
    > OpenJDK 17 下载地址：  
    > https://jdk.java.net/17/  
  
## 阿里巴巴
  * [【阿里巴巴-王超】消灭 Java 代码的“坏味道”](https://mp.weixin.qq.com/s?__biz=MzU4NzU0MDIzOQ==&mid=2247487714&idx=1&sn=8f9de656a4abe236b16415e6ecaa5f9d)
  * [《阿里巴巴 Java 开发手册 1.7.0 嵩山版》2020-08-03 PDF（请新标签页打开）](https://ghost.oss.sherlocky.com/learning/java/Java%E5%BC%80%E5%8F%91%E6%89%8B%E5%86%8C-%E5%B5%A9%E5%B1%B1%E7%89%88-1.7.0.pdf)
  > 官方主页：https://developer.aliyun.com/topic/java2020
  * [《Java开发手册》解读：大整数传输为何禁用Long类型?](https://mp.weixin.qq.com/s/ftG0sRBLkKfwXQas7Ee0uQ)
  * [《Java开发手册（嵩山版）灵魂15问》解读手册](https://developer.aliyun.com/article/769906)
    > [PDF版（请新标签页打开）](https://ghost.oss.sherlocky.com/learning/java/Java%E5%BC%80%E5%8F%91%E6%89%8B%E5%86%8C-%E5%B5%A9%E5%B1%B1%E7%89%88-%E7%81%B5%E9%AD%8215%E9%97%AE.pdf)
  * [Hollis-Java工程师成神之路](http://hollischuang.gitee.io/tobetopjavaer/#/menu)
    > [PDF版（请新标签页打开）](https://ghost.oss.sherlocky.com/learning/java/Java%E5%B7%A5%E7%A8%8B%E5%B8%88%E6%88%90%E7%A5%9E%E4%B9%8B%E8%B7%AF.pdf)
  
  * [阿里巴巴Java开发手册IDE插件](https://yq.aliyun.com/articles/224817?utm_content=m_32519)
  * [JAVA核心知识点整理.pdf](https://ghost.oss.sherlocky.com/learning/java/JAVA%E6%A0%B8%E5%BF%83%E7%9F%A5%E8%AF%86%E7%82%B9%E6%95%B4%E7%90%86.pdf)
  
## 反射
  * [Class.forName和ClassLoader的区别](https://www.cnblogs.com/jimoer/p/9185662.html)
  
## 重写和重载
  * [细说 Java Overload 与 Override 差别](https://mp.weixin.qq.com/s?__biz=MjM5NzMyMjAwMA==&mid=2651484817&idx=1&sn=8807daa4aa95d8c044c73c9e860988e6)
  * [英文原文](https://software.rajivprab.com/2019/08/14/nuances-of-overloading-and-overriding-in-java/)

## 接口的默认方法
  > Java 8 新增了接口的默认方法
  * ``super``和``this``在子接口中的使用
    > 由于接口不是类，super和this的使用和类将会产生较大的区别。  
    > 首先我们无法在子接口中使用super，只能使用this。（接口名.super和接口名.this仍旧等价于super和this）  
    > 而对于父接口，我们无法通过super来调用的情况下，我们必须通过**父接口名.super**的方式来调用某个父接口。  
    > 也就是说父接口名.super指向的不是父接口的父接口，而是其本身。  
    > 这是因为一个接口可以继承多个接口，我们无法直接使用super来指代某一个父接口，所以编译器阻止了super这样的用法，即便只继承了一个父接口，
    > 改而使用父接口名.super这样显式的指出哪一个父接口。

## 序列化
  * [【原创】（译）Java 序列化魔法方法及使用示例](https://juejin.im/post/5d7206c5f265da03ab427181)
  * [FastJson稍微使用不当就会导致StackOverflow](https://mp.weixin.qq.com/s?__biz=MzI3NzE0NjcwMg==&mid=2650125098&idx=1&sn=2390567e228e1257af3d4b6090c7065d)
  > - 1、方法名不以get开头
  > - 2、使用@JSONField(serialize = false)修饰目标方法
  > - 3、使用@JSONType修饰该Bean，并ignore掉方法对应的属性名（getXxx -> xxx）
  * [初识Jackson -- 世界上最好的JSON库](https://www.imooc.com/article/306573)
  
  * [JAVA反序列化 - Commons-Collections组件](https://xz.aliyun.com/t/7031)
  > cc链
  * [Dubbo 反序列化高危漏洞探究](https://mp.weixin.qq.com/s/-jIeLJadGg9U1dFHvPw0pw)
  
## 集合
  * 一个普通的对象，能够作为HashMap的key么？
  > 答案显然是**可以**的，但需要注意重写``hashCode``和``equals``方法。如果忘记重写的话，大概率会造成**内存泄漏**。
  * [为什么阿里巴巴禁止在 foreach 循环里进行元素的 remove/add 操作](https://halo.sherlocky.com/archives/java#%E9%98%BF%E9%87%8C%E5%B7%B4%E5%B7%B4%E7%A6%81%E6%AD%A2%E5%9C%A8-foreach-%E5%BE%AA%E7%8E%AF%E9%87%8C%E8%BF%9B%E8%A1%8C%E5%85%83%E7%B4%A0%E7%9A%84-removeadd-%E6%93%8D%E4%BD%9C)
  > 还可以参考：https://mp.weixin.qq.com/s/0NF3dT4hTD2WdFaHFe6b_g
  
  * 正确 remove/add 姿势
    - 1.直接使用普通 for 循环进行操作
      > 普通 for 循环并没有用到 Iterator 的遍历，所以压根就没有进行 fail-fast 的检验。  
    其实存在一个问题，那就是 remove 操作会改变 List 中元素的下标，
    可能存在漏删的情况。
    - 2.直接使用 Iterator 进行操作
    - 3.使用 Java 8 中提供的 filter 过滤
      > Java 8 中可以把集合转换成流，对于流有一种 filter 操作， 可以对原始 Stream 进行某项测试，通过测试的元素被留下来生成一个新 Stream。
    - 4.使用增强 for 循环其实也可以
      > 只要在删除之后，立刻结束循环体，不要再继续进行遍历就可以了，也就是说不让代码执行到下一次的 next 方法。
    - 5.直接使用 fail-safe 的集合类  
    在 Java 中，除了一些普通的集合类以外，还有一些采用了 fail-safe （安全失败）机制的集合类。这样的集合容器在遍历时不是直接在集合内容上访问的，而是先复制原有集合内容，在拷贝的集合上进行遍历。  
    由于迭代时是对原集合的拷贝进行遍历，所以在遍历过程中对原集合所作的修改并不能被迭代器检测到，所以不会触发``ConcurrentModificationException``。  
    基于拷贝内容的优点是避免了``ConcurrentModificationException``，但同样地，迭代器并不能访问到修改后的内容，即：**迭代器遍历的是开始遍历那一刻拿到的集合拷贝**，在遍历期间原集合发生的修改迭代器是不知道的。  
      > 比如： ``ConcurrentLinkedDeque``  
      > ``java.util.concurrent`` 包下的容器都是安全失败，可以在多线程下并发使用，并发修改。

  * [《吊打面试官》系列-HashMap](https://juejin.im/post/5dee6f54f265da33ba5a79c8)
  * [《吊打面试官》系列-ConcurrentHashMap & Hashtable](https://juejin.im/post/5df8d7346fb9a015ff64eaf9)
  * [Java集合框架分析-HashMap](http://www.jianshu.com/p/76f5a3d12c28)
  > HashMap是线程不安全的，其主要体现：
  >1.在jdk1.7中(头插法)，在多线程环境下，扩容时会造成环形链或数据丢失。
  >2.在jdk1.8中(尾插法)，在多线程环境下，会发生数据覆盖的情况。
  * [HashMap中的resize以及死链的情况](https://www.cnblogs.com/wang-meng/p/7582532.html)
   > 头插法(1.7) VS 尾插法(1.8+)
  * [HashMap defaultLoadFactor = 0.75和泊松分布没有关系](https://blog.csdn.net/reliveIT/article/details/82960063)
    > 一家之言，未看明白。。  
    > load factory=0.75的真正原因，在java7、8等中均有注释（这段注释在public class HashMap类定义之前）  
    > 负载因子太小了浪费空间并且会发生更多次数的``resize``，太大了哈希冲突增加会导致性能不好，所以0.75只是一个折中的选择，和泊松分布没有什么关系。
  * [HashMap原理详解，看不懂算我输（附面试题）](https://zhuanlan.zhihu.com/p/127147909)
  * [史上最清晰的红黑树讲解](https://github.com/CarpenterLee/JCFInternals/blob/master/markdown/5-TreeSet%20and%20TreeMap.md)
  * [我画了近百张图来理解红黑树](https://juejin.im/post/5df4aaefe51d45581269a6d2)
  > 左旋、右旋的动画图演示很清晰、易懂
  * [红黑树，超强动静图详解，简单易懂](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483852&idx=1&sn=d878eb9c694143a2e791ee9a491e1c77)
  * [深入浅出的分析 TreeMap](https://mp.weixin.qq.com/s/zqn8C5zD41IkqCxOC2asNA)
  * [红黑树在线动画演示](http://algoanim.ide.sk/index.php?page=showanim&id=63)
  * [Java集合框架分析-ArrayList](http://www.jianshu.com/p/36730a42d51b)
  * [Java集合框架分析-LinkedHashMap](http://www.jianshu.com/p/1182237a1940)
  * [ConcurrentHashMap核心原理，这次彻底给整明白了](https://mp.weixin.qq.com/s/2FjfGPyU6xFryh-8MfAcxQ)
  * [ConcurrentHashMap详解以及get方法保持同步的解释](http://blog.csdn.net/seapeak007/article/details/53409618)
  * [从ConcurrentHashMap的演进看Java多线程核心技术](http://www.jasongj.com/java/concurrenthashmap/)
  * [Java 经典面试题：为什么 ConcurrentHashMap 的读操作不需要加锁？](https://mp.weixin.qq.com/s?__biz=MzUzMTA2NTU2Ng==&mid=2247487215&idx=1&sn=f1772b8c7a290df3a3cf7fab4f1f54bc)
  >1.在1.8中ConcurrentHashMap的``get``操作全程不需要加锁，这也是它比其他并发集合比如hashtable、用Collections.synchronizedMap()包装的hashmap;安全效率高的原因之一。
  >2.get操作全程不需要加锁是因为Node的成员val是用volatile修饰的和数组用volatile修饰没有关系。
  >3.数组用volatile修饰主要是保证在数组扩容的时候保证可见性。
  * [并发容器 - 基于SkipList的Map和Set](https://juejin.im/post/58caa1a8ac502e005889d36b)
  * [Java 18 种队列图解，还有比这更好的安排吗？](https://mp.weixin.qq.com/s/__M-DmA4mf4_GLd0ekReIA)

## JMM
  * [Java对象都是在堆上分配空间吗？答案竟然是...](https://mp.weixin.qq.com/s?__biz=MzU1NTkwODE4Mw==&mid=2247485006&idx=1&sn=85d6fa16c224fe93cf167f4d44d432ee)
  > 热点监测、JIT编译(Just In Time)、逃逸分析、标量替换、栈上分配
  * [面试必问的 volatile，你真的理解了吗](https://mp.weixin.qq.com/s?__biz=MzU1NTkwODE4Mw==&mid=2247484982&idx=2&sn=be0c717ffe0974a9323fed651b893128)
  * [Java并发编程：volatile关键字解析](http://www.importnew.com/18126.html)
  
## JVM
  * [深入了解Java之类加载和案例分析](http://itfeifei.win/2017/03/14/%E6%B7%B1%E5%85%A5%E4%BA%86%E8%A7%A3Java%E4%B9%8B%E7%B1%BB%E5%8A%A0%E8%BD%BD%E5%92%8C%E6%A1%88%E4%BE%8B%E5%88%86%E6%9E%90/)
  * [面试官问类加载器的双亲委派，你应该这样回答，100分！](https://mp.weixin.qq.com/s?__biz=MzU5ODUwNzY1Nw==&mid=2247484936&idx=1&sn=32cb67042521bceb94ee5163e3e513e8)
  * [死磕Java内部类（一篇就够）](https://juejin.im/post/5d0821315188254c434686c8)
  * [可能是把Java内存区域讲的最清楚的一篇文章](https://github.com/Snailclimb/JavaGuide/blob/master/docs/java/jvm/Java%E5%86%85%E5%AD%98%E5%8C%BA%E5%9F%9F.md)
  * [【简单易懂-来自深入理解Java虚拟机】咱们从头到尾说一次 Java 垃圾回收](https://mp.weixin.qq.com/s?__biz=MzU4NzU0MDIzOQ==&mid=2247487045&idx=1&sn=17893a72e5567b6fefd4f11c92eecca6)
  * [Java垃圾回收复制算法为什么要有两个Survivor](https://www.jianshu.com/p/a5fd5bf93d26?utm_campaign=haruki&utm_content=note&utm_medium=reader_share&utm_source=weixin&from=singlemessage&isappinstalled=0)
  * [深入了解Java之虚拟机内存](http://itfeifei.win/2017/03/13/%E6%B7%B1%E5%85%A5%E4%BA%86%E8%A7%A3Java%E4%B9%8B%E8%99%9A%E6%8B%9F%E6%9C%BA%E5%86%85%E5%AD%98/)
  * [什么是主内存，工作内存;可见性;原子性；有序性](https://juejin.im/post/5d16a633e51d455a2f2202a3)
  * [OutOfMemoryError系列（2）: GC overhead limit exceeded](https://blog.csdn.net/renfufei/article/details/77585294)
  * [jvm优化必知系列——监控工具](https://my.oschina.net/u/1859679/blog/1552290)
  * [一次元空间内存泄露分析记录](https://mp.weixin.qq.com/s/94twrZuIob5_mmC27FoI5g)
    > JDK 1.8 后，Hotspot 虚拟机已经移除了永久代，使用了元空间代替，``-XX:PermSize=256m -XX:MaxPermSize=512m``配置的是永久代的内存空间，这两个参数对于1.8就是过期的参数，**无效**。

### 垃圾回收（GC）
  * [搞定JVM垃圾回收就是这么简单.md](https://github.com/Snailclimb/JavaGuide/blob/master/docs/java/jvm/JVM%E5%9E%83%E5%9C%BE%E5%9B%9E%E6%94%B6.md)
  * [老大难的GC原理及调优，这下全说清楚了](https://juejin.im/post/5b6b986c6fb9a04fd1603f4a)
  * [7种 JVM 垃圾收集器特点、优劣势及使用场景(多图)](https://mp.weixin.qq.com/s?__biz=MzI4ODQ3NjE2OA==&mid=2247485429&idx=1&sn=66ffb35d073012b73eba12d3f6337388)
  * [jvm优化—— 图解垃圾回收](https://my.oschina.net/u/1859679/blog/1548866)   
  * [不可错过的CMS学习笔记](https://mp.weixin.qq.com/s/-yqJa4dOyzLaK_tJ1x9E7w)
  * [既然JVM有Full GC，为什么还会出现OutOfMemoryError?](https://mp.weixin.qq.com/s?__biz=MzIwMzY1OTU1NQ==&mid=2247487133&idx=2&sn=f0eaffdbec9852d5cf2bd19d12703b29)   
  * [Java中9种常见的CMS GC问题分析与解决](https://tech.meituan.com/2020/11/12/java-9-cms-gc.html)
  * [java8添加并查看GC日志(ParNew+CMS)](https://segmentfault.com/a/1190000021453229)
  * [一次YoungGC过慢排查](https://www.jianshu.com/p/4afabaa2b390)
  * --
  * [46张PPT弄懂JVM、GC算法和性能调优！](https://mp.weixin.qq.com/s/NlrZHEQ7ujb0lYCc0opIrA)
    > [下载ppt戳我](https://ghost.oss.sherlocky.com/halo/JVM%E4%BD%93%E7%B3%BB%E7%BB%93%E6%9E%84%E4%B8%8EGC%E8%B0%83%E4%BC%98.pptx-halo)
  * [jvm：垃圾回收器GC搭配推荐及其常用调优参数](https://blog.csdn.net/qq_42709262/article/details/85092208)
    > G1 即支持新生代又支持老年代，目标是取代 CMS（CMS默认搭配的新生代收集器是ParNew）
    > 还有来自 JDK11 的 ZGC
    > 还有来自 JDK12 的 Shenandoah 
    > ![yongGC](https://ghost.oss.sherlocky.com/halo/yongGC_1631787695766.png-halo)
    > ![oldGC](https://ghost.oss.sherlocky.com/halo/oldGC_1631787690143.png-halo)
  * [G1垃圾回收Region数量变化很大，并且周期性变化](https://heapdump.cn/question/249193)
    > CMS 正式退出历史舞台，G1 正式接棒，ZGC 蓄势待发。
    > 在GC 算法的选择上，目前来看 G1 还是最佳的选择，ZGC 因为有内存占用被 OS 标记过高（三倍共享内存）虚高的问题，进程可能被 OOM-killer 杀掉。
    > G1不要设置新生代和老年代的大小，有新生代自适应策略，会自适应调整新生代的大小。
  * 吞吐量和低延迟的平衡
    > 吞吐量 = CPU在用户应用程序运行的时间 / （CPU在用户应用程序运行的时间 + CPU垃圾回收的时间）
    > 响应时间 = 平均每次的GC的耗时
    >
    > 堆内存增大，gc一次能处理的数量变大，吞吐量大；但是gc一次的时间会变长，导致后面排队的线程等待时间变长；
    > 相反，如果堆内存小，gc一次时间短，排队等待的线程等待时间变短，延迟减少，但一次请求的数量变小（并不绝对符合）。无法同时兼顾，是吞吐优先还是响应优先，这是一个需要权衡的问题。
    >
    > 业务系统，延迟敏感的推荐CMS；
    > 大内存服务，要求高吞吐的，采用G1回收器！
    >
    > 可参考文章：[阿里：每天100w次登陆请求, 8G 内存该如何设置JVM参数？](https://mp.weixin.qq.com/s/HCOeY2yNyHI0EukBNCzsdA)
  * [Shenandoah GC：一个来自JDK12的全新并发压缩垃圾回收器_Java_老男孩的技术博客_51CTO博客_shenandoah](https://blog.51cto.com/u_14230003/2435438)
    > Shenandoah 是一个对那些更看重响应性和可预测短暂停顿的应用来说，更合适的GC算法。它的目标不是要解决所有JVM的停顿问题。
    > Shenandoah 就是这样一个OpenJDK为更近这个目标而设计的开源、低停顿时间的垃圾回收器。
    > Zing/Azul是一个没有停顿的垃圾收集器，但是不会贡献给OpenJDK。
    > 基于colored pointers设计的ZGC也是一个拥有很低停顿时间的垃圾收集器，Shenandoah期望能与之一战。
    > G1很多工作都是并行或者并发的，但是evacuation阶段不能并发执行。
    > CMS能并发标记，但是它执行年轻代拷贝时，需要STW，并且不会压缩老年代，这就会导致花费更多时间来管理老年代中的可用空间以及碎片问题。
  
## 锁
  * [面试官问：说说你对 Java 中锁以及 sychronized 实现机制的理解](https://blog.yoodb.com/yoodb/article/detail/1600)
  * [Java性能之synchronized锁的优化](https://www.bbsmax.com/A/l1dyZB69ze/)
  * [Synchronized 关键字使用、底层原理、JDK1.6 之后的底层优化](https://zhuanlan.zhihu.com/p/47692708)  
  * [看了``Synchronized``源码，请别和我说它慢](https://mp.weixin.qq.com/s/P2Q1SSdT9dFZSAqhjfdQ-A)
  * [synchronized锁字符串问题 + String.intern()解决 + google的Interners解决 java单机锁](https://blog.csdn.net/qq_35493807/article/details/106024468)
  * [使用 Google Guava Striped 实现基于 Key 的并发锁](https://yanbin.blog/google-guava-striped-key-based-fine-grain-locks/)
  * [Java 8的StampedLock](https://www.jdon.com/idea/java/java-8-stampedlock.html)
    > StampedLock要比ReentrantReadWriteLock更加廉价，也就是消耗比较小
  
## 并发
  * [Java8 和 Java 9中并发工具的改变](https://colobu.com/2018/03/12/Concurrency-Utilities-Enhancements-in-Java-8-Java-9/)
  * [浅析LongAdder](https://www.jianshu.com/p/22d38d5c8c2a)
    > LongAdder 并不能替代 AtomicLong
    > LongAdder 适合的场景是统计求和计数，而且LongAdder 基本只提供了add方法，而AtomicLong还具有cas方法。
  * [[译]20个使用 Java CompletableFuture的例子](https://colobu.com/2018/03/12/20-Examples-of-Using-Java%E2%80%99s-CompletableFuture/)
  * [并发 VS 并行](https://cloud.tencent.com/developer/article/1424249)
    > 并发，指的是多个事情，在同一时间段内同时发生了。  
    > 并行，指的是多个事情，在同一时间点上同时发生了。  
    > 
    > 并发的多个任务之间是互相抢占资源的。  
    > 并行的多个任务之间是不互相抢占资源的。  
    > 
    > 只有在多CPU的情况中，才会发生并行。否则，看似同时发生的事情，其实都是并发执行的。
  
## 多线程
  * [【电子书】深入浅出Java多线程](http://concurrent.redspider.group/article/01/1.html)
    > 备用地址：https://redspider.gitbook.io/concurrent/

  * [并发Bug之源有三，请睁大眼睛看清它们](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483941&idx=1&sn=d700824e4039cc487ea930857ec2b5c1)
  * [可见性有序性，Happens-before来搞定](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483947&idx=1&sn=3e8024b80dcccb36747b4b885e21cd69)
  * [解决原子性问题？你首先需要的是宏观理解](https://mp.weixin.qq.com/s?__biz=Mzg3NjIxMjA1Ng==&mid=2247483951&idx=1&sn=e3dc49445b430cf3b6f9b0202af2f7a8)

  * [Java 线程状态之 WAITING](https://my.oschina.net/goldenshaw/blog/802620)
  * [Java 线程状态之 RUNNABLE](https://my.oschina.net/goldenshaw/blog/705397)
  * [计算机程序的思维逻辑 (75) - 并发容器 - 基于 SkipList 的 Map 和 Set](https://juejin.im/post/58caa1a8ac502e005889d36b)

  * [JAVA多线程系列目录（43篇）](http://www.cnblogs.com/skywang12345/p/java_threads_category.html)
  * [【Java 并发笔记】Unsafe 相关整理](https://www.jianshu.com/p/2e5b92d0962e)
  * [Thread详解](https://www.cnblogs.com/waterystone/p/4920007.html)
  * [一文搞懂 ThreadLocal 原理](https://mp.weixin.qq.com/s?__biz=MzU1NTkwODE4Mw==&mid=2247485019&idx=2&sn=979554c738be748c771050f04ebc7ef7)  
    > ThreadLocal 的特性也导致了应用场景比较广泛，主要的应用场景如下：
    > - 1.线程间数据隔离，各线程的 ThreadLocal 互不影响
    > - 2.方便同一个线程使用某一对象，避免不必要的参数传递
    > - 3.全链路追踪中的 traceId 或者流程引擎中上下文的传递一般采用 ThreadLocal
    > - 4.Spring 事务管理器采用了 ThreadLocal
    > - 5.Spring MVC 的 RequestContextHolder 的实现使用了 ThreadLocal

  * [ThreadLocal/Redis Hash 实现可重入分布式锁](https://zhuanlan.zhihu.com/p/148342738)
    > ``private static ThreadLocal<Map<String, Integer>> LOCKS = ThreadLocal.withInitial(HashMap::new);``
    
  * [Callable、Future、FutureTask](https://mp.weixin.qq.com/s/qoZ9zGzROIDvD8Idyvm3XQ)
    > 线程可能的状态转换：
    > - 1.NEW -> COMPLETING -> NORMAL  //执行过程顺利完成
    > - 2.NEW -> COMPLETING -> EXCEPTIONAL //执行过程出现异常
    > - 3.NEW -> CANCELLED // 执行过程中被取消
    > - 4.NEW -> INTERRUPTING -> INTERRUPTED //执行过程中，线程被中断
    > 两个中间状态都表示一种瞬时状态
    > ![](https://ghost.oss.sherlocky.com/halo/thread_state_transitions_1595066249765.png-halo)
  
  * [一个线程池中的线程异常了，那么线程池会怎么处理这个线程?](https://www.cnblogs.com/fanguangdexiaoyuer/p/12332082.html)
    > 当一个线程池里面的线程异常后:  
    > - 1、当执行方式是execute时,可以看到堆栈异常的输出
    > 原因：ThreadPoolExecutor.runWorker()方法中，task.run()，即执行我们的方法，如果异常的话会throw x;所以可以看到异常。
    > - 2、当执行方式是submit时,堆栈异常没有输出。但是调用Future.get()方法时，可以捕获到异常
    > 原因：ThreadPoolExecutor.runWorker()方法中，task.run()，其实还会继续执行FutureTask.run()方法，再在此方法中c.call()调用我们的方法，
    > 如果报错是setException()，并没有抛出异常。当我们去get()时，会将异常抛出。
    > - 3、不会影响线程池里面其他线程的正常执行
    > - 4、线程池会把这个线程移除掉，并创建一个新的线程放到线程池中
    > 当线程异常，会调用ThreadPoolExecutor.runWorker()方法最后面的finally中的processWorkerExit()，会将此线程remove，并重新addworker()一个线程。

## AQS  
  * [Java并发之AQS详解](https://www.cnblogs.com/waterystone/p/4920797.html)
  * [AQS - AbstractQueuedSynchronizer超详细原理解析](https://mp.weixin.qq.com/s?__biz=Mzg2NjE5NDQyOA==&mid=2247483778&idx=1&sn=1217b9ee2ac616678693db2c18db7bf6)
  * [画了35张图就是为了让你深入 AQS](https://mp.weixin.qq.com/s/Ix7eus2R7QcvvWAfFyeAdQ)
  * [AQS 原理以及 AQS 同步组件总结](https://javaguide.cn/java/concurrent/aqs.html#aqs-%E7%AE%80%E5%8D%95%E4%BB%8B%E7%BB%8D)
    > - 底层使用了模板方法模式，可参考：[用Java8改造后的模板方法模式真的是yyds!](https://mp.weixin.qq.com/s/zpScSCktFpnSWHWIQem2jg)
    > - ReentrantReadWriteLock：读写锁，可以保证多个线程可以同时读，所以在读操作远大于写操作的时候，读写锁就非常有用了。
    >   - 内部维护两个锁, 一个是写锁, 另外一个是读锁. 通过将读写锁分离, 在读多写少的情况下, 更够提高程序的并发程度。
    >   - ReentrantReadWriteLock的伸缩性要好于ReentrantLock. 在读多写少的情况下, 应该使用ReentrantReadWriteLock更为合适.
    >   - ReentrantReadWriteLock只支持锁降级, 不支持锁升级. 因为锁升级有可能会出现条件竞争. 
    >   - 由于读锁是可以被多个线程持有的, 如果进行锁升级的话, 当写线程改变共享变量的状态时, 其他读线程有可能感知不到.
    > - ReentrantLock
    > - Semaphore
    > - CountDownLatch 倒计时器：两种典型用法
    >   - 1、某一线程在开始运行前等待 n 个线程执行完毕。
    >   - 2、实现多个线程开始执行任务的最大并行性。
    > - CyclicBarrier(循环栅栏)：CountDownLatch 的实现是基于 AQS 的，而 CycliBarrier 是基于 ReentrantLock(ReentrantLock 也属于 AQS 同步器)和 Condition 的。
  * [从ReentrantLock的实现看AQS的原理及应用](https://javaguide.cn/java/concurrent/reentrantlock.html#aqs-%E7%AE%80%E5%8D%95%E4%BB%8B%E7%BB%8D)
  
## 线程池  
  * [线程池没你想的那么简单](https://juejin.im/post/5ce1f3b6f265da1ba2522f62)
  * [深入理解java线程池—ThreadPoolExecutor](http://www.jianshu.com/p/ade771d2c9c0)  
  * [java线程池ThreadPoolExecutor八种拒绝策略浅析](http://www.kailing.pub/article/index/arcid/255.html)
  * [你知道如何安全正确的关闭线程池吗？](https://mp.weixin.qq.com/s?__biz=MzU3NzczMTAzMg==&mid=2247485650&idx=1&sn=9182c3d618ce868999025f1875b3c370)
  * [面试官：为什么《阿里巴巴Java开发手册》上要禁止使用Executors来创建线程池](https://juejin.im/post/5dd72e226fb9a04c352df756)
  * [为什么阿里巴巴要禁用Executors创建线程池？](https://juejin.im/post/5dc41c165188257bad4d9e69)
  > 推荐使用 guava 的 ThreadFactoryBuilder 来创建线程池
  * [线程池submit()方法提交任务可能没有异常抛出](https://mp.weixin.qq.com/s/TQGtNpPiTypeKd5kUnfxEw)
  > 
  ```java
  ThreadFactory namedThreadFactory = new ThreadFactoryBuilder()
                .setNameFormat("judge-pool-%d")
                .setUncaughtExceptionHandler((thread, throwable)-> logger.error("ThreadPool {} got exception", thread,throwable))
                .build();
  ```
  * [合理的设置线程池队列长度](https://blog.csdn.net/huangshanchun/article/details/78567501)
  * [线程池最佳线程数量到底要如何配置？](https://mp.weixin.qq.com/s/MPsUd0sy0yojcUoSYl8B2A)
  * [Java线程池实现原理及其在美团业务中的实践](https://tech.meituan.com/2020/04/02/java-pooling-pratice-in-meituan.html)
    > 美团并没有开源，可以参考其他开源实现：  
    > https://zhuanlan.zhihu.com/p/149138818  
    > https://github.com/yinjihuan/kitty/tree/master/kitty-dynamic-thread-pool/src/main/java/com/cxytiandi/kitty/threadpool
  * [ThreadPoolExecutor-动态调节线程池大小](https://blog.csdn.net/u013887008/article/details/116354869)
  * 基于美团线程池实践的启发
    - 考虑到在实际应用中我们获取并发性的场景主要是两种：
	     - （1）并行执行子任务，提高响应速度。这种情况下，应该使用同步队列，没有什么任务应该被缓存下来，而是应该立即执行。
	     - （2）并行执行大批次任务，提升吞吐量。这种情况下，应该使用有界队列，使用队列去缓冲大批量的任务，队列容量必须声明，防止任务无限制堆积。
      > 所以线程池只需要提供corePoolSize、maximumPoolSize，workQueue这三个关键参数的配置，它们最大程度地决定了线程池的任务分配和线程分配策略。  
      > 并且提供两种队列的选择，就可以满足绝大多数的业务需求，Less is More。
    - 动态修改线程池主要参数。（在Java线程池留有高扩展性的基础上，封装线程池，允许线程池监听同步外部的消息，根据消息进行修改配置）
      > 
      ```java
       //先设置maxPoolSize,不然会设置失败（主要看修改后和修改前池大小的比较，修改时最大数不能小于核心数）
       threadPoolExecutor.setMaximumPoolSize(10);	
       threadPoolExecutor.setCorePoolSize(10);
       threadPoolExecutor.setKeepAliveTime();
       threadPoolExecutor.setRejectedExecutionHandler();
       BlockingQueue<Runnable> queue = threadPoolExecutor.getQueue();
       if (queue instanceof ResizableCapacityLinkedBlockIngQueue) {
           // LinkedBlockingQueue中没有原始方法去设置队列长度，可以copy 一个LinkedBlockingQueue, 修改capacity
           ((ResizableCapacityLinkedBlockIngQueue<Runnable>) queue).setCapacity(newQueueCapacity);
       }
      ```
      ```java
	    private static void changeExecutorPoolSize(ThreadPoolExecutor executor, int newCoreSize, int newMaximumSize) {
		if (newCoreSize > newMaximumSize) {
		    log.error("核心池大小不能超过允许的最大线程数");
		    return;
		}
		if (newMaximumSize <= 0) {
		    log.error("最大线程数不能为0或小于0");
		    return;
		}
		if (newCoreSize < 0) {
		    log.error("核心线程数不能小于0");
		    return;
		}
		int oldCoreSize = executor.getCorePoolSize();
		int oldMaximumSize = executor.getMaximumPoolSize();
		if (newCoreSize == oldCoreSize && newMaximumSize == oldMaximumSize) {
		    log.info("线程池大小配置未变更，忽略~");
		    return;
		}
		if (newMaximumSize < oldMaximumSize) {
		    // 缩小时，先设置corePoolSize，后设置maxPoolSize
		    executor.setCorePoolSize(newCoreSize);
		    executor.setMaximumPoolSize(newMaximumSize);
		    return;
		}
		// 扩大时，先设置maxPoolSize，后设置corePoolSize
		executor.setMaximumPoolSize(newMaximumSize);
		executor.setCorePoolSize(newCoreSize);
	    }
      ```
      ```java
       /**
       * ResizableCapacityLinkedBlockIngQueue copy from LinkedBlockingQueue
       * 修改 capacity 大小
       * @param newCapacity
       */
       public synchronized void setCapacity(int newCapacity) {
           if (newCapacity < capacity) {
               throw new IllegalStateException("队列长度设置异常");
           }
           this.capacity = newCapacity;
       }
      ```
    - 线程池监控和告警
  
## CompletableFuture & ForkJoinPool & parallelStream
- [CompletableFuture 使用详解](https://www.jianshu.com/p/6bac52527ca4)
- [Java 8 CompletableFuture 教程](https://segmentfault.com/a/1190000014479792)
- [ForkJoinPool](https://www.jianshu.com/p/a152c0a0d2d0)
- [parallelStream与ForkJoinPool的二三事](https://www.vergessen.top/article/v/22552932698734266)
- [Stream的collect方法是怎么保证线程安全的](https://lijf.me/2019/12/04/how-stream-makes-colloct-thread-safe/)
  
## 动态代理
  * [java中动态代理实现机制](https://yq.aliyun.com/articles/35985)
  * [CGLib动态代理原理及实现](https://my.oschina.net/mifans/blog/783470)
  * [Spring AOP动态代理原理与实现方式 （转）](http://www.tuicool.com/articles/jMzmQj)
  
## 泛型
 * [JAVA 泛型中的通配符 T，E，K，V，?](https://juejin.cn/post/6844903917835419661)
 
## 高性能
* [高性能 Disruptor——消除伪共享](https://jitwxs.cn/13836b16.html)
  > 例如：``Thread``类中``@sun.misc.Contended("tlr")``的使用
* [高性能队列——Disruptor](https://tech.meituan.com/2016/11/18/disruptor.html)

## 高阶
* [Java即时编译器原理解析及实践](https://tech.meituan.com/2020/10/22/java-jit-practice-in-meituan.html)
* [扒了 Java 的皮，看见它的心](https://mp.weixin.qq.com/s/zBfvjq3gry2zsMoMir6oZA)
  - jclasslib javap：看见字节码
  - strace：看见系统调用
  - HSDIS + JITWATCH：看见机器码（汇编）
  - openJDK：看见 native 方法
  - JOL：看见对象
  - fastthread：看见线程
    > [Java Thread Dump Analyzer](https://fastthread.io/)
  - JProfile：看见运行时的各种状态

## Docker虚拟化
* [性能优化 - Docker 容器中的 Java 内存使用分析](https://cloud.tencent.com/developer/article/1887538)

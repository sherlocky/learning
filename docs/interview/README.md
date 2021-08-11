# 面试
* [【防坑指南】从写简历，到面试和谈薪酬](https://mp.weixin.qq.com/s?__biz=MzI4Njg5MDA5NA==&mid=2247486916&idx=1&sn=887a3ee2b5a17bc4a773d2af823de954)
* [Snailclimb/JavaGuide【Java学习+面试指南】 8W+ Star](https://github.com/Snailclimb/JavaGuide)
  > 一份涵盖大部分Java程序员所需要掌握的核心知识。[博客版地址](https://snailclimb.top/JavaGuide/#/)
* [【敖丙】5W字的后端面经（持续更新）](https://juejin.im/post/5ec0ff4a6fb9a043271c76e9)
  > [微信版地址](https://mp.weixin.qq.com/s/gBr3UfC1HRcw4U-ZMmtRaQ)

* [【中华红杉】互联网 Java 工程师进阶知识完全扫盲](https://github.com/doocs/advanced-java)
  > [github博客版地址](https://doocs.github.io/advanced-java/)
  
* [2019年最新总结，阿里，腾讯，百度，美团，头条等技术面试题目，以及答案，专家出题人分析汇总。](https://github.com/0voice/interview_internal_reference)  
* [2017年阿里内推一面面经（不断更新）](https://juejin.im/post/58cfb1da128fe1006c9b36a1)
* [经典面试题：从 URL 输入到页面展现到底发生什么？](https://yq.aliyun.com/articles/691698)

## 学习路线
* [大厂java面试考点/学习路线](https://www.processon.com/view/5e86b713e4b0bf3ebcf4e376#map)

## 精进
* [写给工程师的十条精进原则](https://tech.meituan.com/2018/08/16/10-principles-for-engineers.html)

## 各种锁
* [面试官：你说说互斥锁、自旋锁、读写锁、悲观锁、乐观锁的应用场景](https://cloud.tencent.com/developer/article/1700079)
  > 最底层的两种就是「互斥锁和自旋锁」，有很多高级的锁都是基于它们实现的，可以认为它们是各种锁的地基。
  > - 互斥锁加锁失败后，线程会释放 CPU ，给其他线程；
  > - 自旋锁加锁失败后，线程会忙等待，直到它拿到锁；
  > 
  > 前面提到的**互斥锁**、**自旋锁**、**读写锁**，都是属于悲观锁。  
  > 
  > **悲观锁**做事比较悲观，它认为多线程同时修改共享资源的概率比较高，于是很容易出现冲突，所以访问共享资源前，先要上锁。
  > 那相反的，如果多线程同时修改共享资源的概率比较低，就可以采用乐观锁。
  > 
  > **乐观锁**做事比较乐观，它假定冲突的概率很低，它的工作方式是：先修改完共享资源，再验证这段时间内有没有发生冲突，如果没有其他线程在修改资源，那么操作完成，如果发现有其他线程已经修改过这个资源，就放弃本次操作。
  > 放弃后如何重试，这跟业务场景息息相关，虽然重试的成本很高，但是冲突的概率足够低的话，还是可以接受的。
  > 另外，你会发现乐观锁全程并没有加锁，所以它也叫**无锁编程**。

# Big-Data-Interview
大数据面试知识点，多为网上公开资料，留以自用。
## 目录
- [Java基础篇](#Java基础篇)
    - [语言基础](#语言基础)
    - [锁](#锁)
    - [多线程](#多线程)
    - [并发容器](#并发容器)
- [JVM](#JVM)
    - [JVM内存结构](#JVM内存结构)
    - [堆和栈区别](#堆和栈区别)
    - [Java内存模型](#Java内存模型)
    - [垃圾回收](#垃圾回收)
    - [Java对象模型](#Java对象模型)
    - [HotSpot](#HotSpot)
    - [虚拟机性能监控与故障处理工具](#虚拟机性能监控与故障处理工具)
    - [类加载机制](#类加载机制)
- [Linux、IO](#Linux、IO)
    - [Linux基础](#Linux基础)
    - [IO](#IO)
- [分布式](#分布式)
    - [分布式理论](#分布式理论)
- [面试](#面试)
    - [计算机网络](#计算机网络)
    - [Spring](#Spring)
    - [Redis](#Redis)

## Java基础篇
### 语言基础
* #### [Java的面向对象](1.%20Java基础篇/1.%20语言基础/1.%20Java的面向对象.md)
* #### [Java语言的三大特征：封装、继承和多态](1.%20Java基础篇/1.%20语言基础/2.%20Java语言的三大特征：封装、继承和多态.md)
* #### [Java语言数据类型](1.%20Java基础篇/1.%20语言基础/3.%20Java语言数据类型.md)
* #### [Java的自动类型转换，强制类型转换](1.%20Java基础篇/1.%20语言基础/4.%20Java的自动类型转换，强制类型转换.md)
* #### [String的不可变性、虚拟机的常量池中的String字符串、String.intern()的底层原理](1.%20Java基础篇/1.%20语言基础/5.%20String的不可变性、虚拟机的常量池中的String字符串、String.intern()的底层原理.md)
* #### [Java语言中的关键字：final](1.%20Java基础篇/1.%20语言基础/6.%20Java语言中的关键字：final.md)
* #### [Java语言中的关键字：static](1.%20Java基础篇/1.%20语言基础/7.%20Java语言中的关键字：static.md)
* #### [Java语言中的关键字：transient](1.%20Java基础篇/1.%20语言基础/8.%20Java语言中的关键字：transient.md)
* #### [Java语言中的关键字：instanceof](1.%20Java基础篇/1.%20语言基础/9.%20Java语言中的关键字：instanceof.md)
* #### [Java语言中的关键字：volatile](1.%20Java基础篇/1.%20语言基础/10.%20Java语言中的关键字：volatile.md)
* #### [Java语言中的关键字：synchronized](1.%20Java基础篇/1.%20语言基础/11.%20Java语言中的关键字：synchronized.md)
* #### [Java中常用的集合类：ArrayList](1.%20Java基础篇/1.%20语言基础/12.%20Java中常用的集合类：ArrayList.md)
* #### [Java中常用的集合类：LinkedList](1.%20Java基础篇/1.%20语言基础/13.%20Java中常用的集合类：LinkedList.md)
* #### [Java中常用的集合类：SynchronizedList](1.%20Java基础篇/1.%20语言基础/14.%20Java中常用的集合类：SynchronizedList.md)
* #### [Java中常用的集合类：HashMap](1.%20Java基础篇/1.%20语言基础/15.%20Java中常用的集合类：HashMap.md)
* #### [Java中常用的集合类：Hashtable](1.%20Java基础篇/1.%20语言基础/16.%20Java中常用的集合类：Hashtable.md)
* #### [Java中常用的集合类：ConcurrentHashMap](1.%20Java基础篇/1.%20语言基础/17.%20Java中常用的集合类：ConcurrentHashMap.md)
* #### [动态代理的实现方式](1.%20Java基础篇/1.%20语言基础/18.%20动态代理的实现方式.md)
### 锁
* #### [CAS](1.%20Java基础篇/2.%20锁/1.%20CAS.md)
* #### [乐观锁与悲观锁](1.%20Java基础篇/2.%20锁/2.%20乐观锁与悲观锁.md)
* #### [分布式锁](1.%20Java基础篇/2.%20锁/3.%20分布式锁.md)
* #### [偏向锁](1.%20Java基础篇/2.%20锁/4.%20偏向锁.md)
* #### [轻量级锁](1.%20Java基础篇/2.%20锁/5.%20轻量级锁.md)
* #### [monitor](1.%20Java基础篇/2.%20锁/6.%20monitor.md)
* #### [锁消除和锁粗化](1.%20Java基础篇/2.%20锁/7.%20锁消除和锁粗化.md)
* #### [自旋锁](1.%20Java基础篇/2.%20锁/8.%20自旋锁.md)
* #### [可重入锁](1.%20Java基础篇/2.%20锁/9.%20可重入锁.md)
* #### [阻塞锁](1.%20Java基础篇/2.%20锁/10.%20阻塞锁.md)
* #### [死锁](1.%20Java基础篇/2.%20锁/11.%20死锁.md)
* #### [CountDownLatch](1.%20Java基础篇/2.%20锁/12.%20CountDownLatch.md)
* #### [CyclicBarrier](1.%20Java基础篇/2.%20锁/13.%20CyclicBarrier.md)
* #### [Semaphore](1.%20Java基础篇/2.%20锁/14.%20Semaphore.md)
### 多线程
* #### [并发和并行的区别、进程与线程的区别](1.%20Java基础篇/3.%20多线程/1.%20并发和并行的区别、进程与线程的区别.md)
* #### [线程的实现](1.%20Java基础篇/3.%20多线程/2.%20线程的实现.md)
* #### [线程的状态](1.%20Java基础篇/3.%20多线程/3.%20线程的状态.md)
* #### [线程的优先级](1.%20Java基础篇/3.%20多线程/4.%20线程的优先级.md)
* #### [线程调度](1.%20Java基础篇/3.%20多线程/5.%20线程调度.md)
* #### [守护线程](1.%20Java基础篇/3.%20多线程/6.%20守护线程.md)
* #### [自己设计线程池](1.%20Java基础篇/3.%20多线程/7.%20自己设计线程池.md)
* #### [submit()和execute()](1.%20Java基础篇/3.%20多线程/8.%20submit()和execute().md)
* #### [线程池原理](1.%20Java基础篇/3.%20多线程/9.%20线程池原理.md)
* #### [为什么不允许使用Executors创建线程池](1.%20Java基础篇/3.%20多线程/10.%20为什么不允许使用Executors创建线程池.md)
* #### [ThreadLocal变量](1.%20Java基础篇/3.%20多线程/11.%20ThreadLocal变量.md)
* #### [ThreadPoolExecutor创建线程池](1.%20Java基础篇/3.%20多线程/12.%20ThreadPoolExecutor创建线程池.md)
* #### [线程池关闭的方式](1.%20Java基础篇/3.%20多线程/13.%20线程池关闭的方式.md)
### 并发容器
* #### [CopyOnWriteArrayList](1.%20Java基础篇/4.%20并发容器/1.%20CopyOnWriteArrayList.md)
* #### [CopyOnWriteArraySet](1.%20Java基础篇/4.%20并发容器/2.%20CopyOnWriteArraySet.md)
* #### [ConcurrentSkipListSet](1.%20Java基础篇/4.%20并发容器/3.%20ConcurrentSkipListSet.md)
* #### [ConcurrentSkipListMap](1.%20Java基础篇/4.%20并发容器/4.%20ConcurrentSkipListMap.md)
* #### [ConcurrentLinkedQueue](1.%20Java基础篇/4.%20并发容器/5.%20ConcurrentLinkedQueue.md)
* #### [ConcurrentLinkedDeque](1.%20Java基础篇/4.%20并发容器/6.%20ConcurrentLinkedDeque.md)
* #### [ArrayBlockingQueue](1.%20Java基础篇/4.%20并发容器/7.%20ArrayBlockingQueue.md)
* #### [LinkedBlockingQueue](1.%20Java基础篇/4.%20并发容器/8.%20LinkedBlockingQueue.md)
* #### [LinkedBlockingDeque](1.%20Java基础篇/4.%20并发容器/9.%20LinkedBlockingDeque.md)
## JVM
### JVM内存结构
* #### [class文件格式](2.%20JVM/1.%20JVM内存结构/1.%20class文件格式.md)
* #### [运行时数据区：堆、栈、方法区](2.%20JVM/1.%20JVM内存结构/2.%20运行时数据区：堆、栈、方法区.md)
* #### [直接内存](2.%20JVM/1.%20JVM内存结构/3.%20直接内存.md)
* #### [运行时常量池](2.%20JVM/1.%20JVM内存结构/4.%20运行时常量池.md)
### 堆和栈区别
* #### [Java中的对象一定在堆上分配吗？](2.%20JVM/2.%20堆和栈区别/1.%20Java中的对象一定在堆上分配吗？.md)
### Java内存模型
* #### [Java内存模型与硬件内存架构关系](2.%20JVM/3.%20Java内存模型/1.%20Java内存模型与硬件内存架构关系.md)
* #### [缓存一致性](2.%20JVM/3.%20Java内存模型/2.%20缓存一致性.md)
* #### [可见性、原子性、顺序性（有序性）](2.%20JVM/3.%20Java内存模型/3.%20可见性、原子性、顺序性（有序性）.md)
* #### [内存屏障](2.%20JVM/3.%20Java内存模型/4.%20内存屏障.md)
* #### [final](2.%20JVM/3.%20Java内存模型/5.%20final.md)
### 垃圾回收
* #### [标记清除](2.%20JVM/4.%20垃圾回收/1.%20标记清除.md)
* #### [引用计数](2.%20JVM/4.%20垃圾回收/2.%20引用计数.md)
* #### [复制算法](2.%20JVM/4.%20垃圾回收/3.%20复制算法.md)
* #### [标记压缩](2.%20JVM/4.%20垃圾回收/4.%20标记压缩.md)
* #### [分代回收](2.%20JVM/4.%20垃圾回收/5.%20分代回收.md)
* #### [增量式回收](2.%20JVM/4.%20垃圾回收/6.%20增量式回收.md)
* #### [GC参数](2.%20JVM/4.%20垃圾回收/7.%20GC参数.md)
* #### [对象存活的判定](2.%20JVM/4.%20垃圾回收/8.%20对象存活的判定.md)
* #### [垃圾收集器](2.%20JVM/4.%20垃圾回收/9.%20垃圾收集器.md)
### Java对象模型
* #### [oop-klass](2.%20JVM/5.%20Java对象模型/1.%20oop-klass.md)
* #### [对象头](2.%20JVM/5.%20Java对象模型/2.%20对象头.md)
### HotSpot
* #### [即时编译器](2.%20JVM/6.%20HotSpot/1.%20即时编译器.md)
* #### [编译优化](2.%20JVM/6.%20HotSpot/2.%20编译优化.md)
### 虚拟机性能监控与故障处理工具
* #### [jps、jstack、jmap、jstat、jconsole、jinfo、jhat](2.%20JVM/7.%20虚拟机性能监控与故障处理工具/1.%20jps、jstack、jmap、jstat、jconsole、jinfo、jhat.md)
* #### [javap](2.%20JVM/7.%20虚拟机性能监控与故障处理工具/2.%20javap.md)
* #### [btrace](2.%20JVM/7.%20虚拟机性能监控与故障处理工具/3.%20btrace.md)
* #### [TProfiler](2.%20JVM/7.%20虚拟机性能监控与故障处理工具/4.%20TProfiler.md)
* #### [Arthas](2.%20JVM/7.%20虚拟机性能监控与故障处理工具/5.%20Arthas.md)
### 类加载机制
* #### [classLoader](2.%20JVM/8.%20类加载机制/1.%20classLoader.md)
* #### [类加载过程](2.%20JVM/8.%20类加载机制/2.%20类加载过程.md)
* #### [双亲委派（破坏双亲委派）](2.%20JVM/8.%20类加载机制/3.%20双亲委派（破坏双亲委派）.md)
* #### [模块化_jboss_modules](2.%20JVM/8.%20类加载机制/4.%20模块化_jboss_modules.md)
* #### [模块化_osgi](2.%20JVM/8.%20类加载机制/5.%20模块化_osgi.md)
* #### [模块化_jigsaw](2.%20JVM/8.%20类加载机制/6.%20模块化_jigsaw.md)
## Linux、IO
### Linux基础
* #### [Linux的常用命令](3.%20Linux、IO/1.%20Linux基础/1.%20Linux的常用命令.md)
* #### [远程登录](3.%20Linux、IO/1.%20Linux基础/2.%20远程登录.md)
* #### [系统目录](3.%20Linux、IO/1.%20Linux基础/3.%20系统目录.md)
* #### [文件和目录操作](3.%20Linux、IO/1.%20Linux基础/4.%20文件和目录操作.md)
* #### [Linux下的权限体系](3.%20Linux、IO/1.%20Linux基础/5.%20Linux下的权限体系.md)
* #### [压缩和打包](3.%20Linux、IO/1.%20Linux基础/6.%20压缩和打包.md)
* #### [Shell脚本的编写](3.%20Linux、IO/1.%20Linux基础/7.%20Shell脚本的编写.md)
* #### [管道操作](3.%20Linux、IO/1.%20Linux基础/8.%20管道操作.md)
### IO
* #### [用户空间以及内核空间](3.%20Linux、IO/2.%20IO/1.%20用户空间以及内核空间.md)
* #### [阻塞、非阻塞、信号驱动式、同步、异步IO](3.%20Linux、IO/2.%20IO/2.%20阻塞、非阻塞、信号驱动式、同步、异步IO.md)
* #### [零拷贝（ZeroCopy）](3.%20Linux、IO/2.%20IO/3.%20零拷贝（ZeroCopy）.md)
* #### [BIO、NIO、AIO](3.%20Linux、IO/2.%20IO/4.%20BIO、NIO、AIO.md)
* #### [缓冲区Buffer](3.%20Linux、IO/2.%20IO/5.%20缓冲区Buffer.md)
* #### [通道Channel](3.%20Linux、IO/2.%20IO/6.%20通道Channel.md)
* #### [反应堆（Reactor）](3.%20Linux、IO/2.%20IO/7.%20反应堆（Reactor）.md)
* #### [选择器（Selector）](3.%20Linux、IO/2.%20IO/8.%20选择器（Selector）.md)
* #### [AIO](3.%20Linux、IO/2.%20IO/9.%20AIO.md)
## 分布式
### 分布式理论
* #### [分布式中的一些基本概念](4.%20分布式/1.%20分布式理论/1.%20分布式系统的一些基本概念.md)
* #### [分布式系统理论基础：一致性、2PC和3PC](4.%20分布式/1.%20分布式理论/2.%20分布式系统理论基础：一致性、2PC和3PC.md)
* #### [分布式系统理论基础：时间、时钟和事件顺序](4.%20分布式/1.%20分布式理论/3.%20分布式系统理论基础：时间、时钟和事件顺序.md)
* #### [分布式系统理论进阶：Paxos](4.%20分布式/1.%20分布式理论/4.%20分布式系统理论进阶：Paxos.md)
* #### [分布式系统理论进阶：Raft、Zab](4.%20分布式/1.%20分布式理论/5.%20分布式系统理论进阶：Raft、Zab.md)
* #### [分布式系统理论进阶：选举、多数派和租约](4.%20分布式/1.%20分布式理论/6.%20分布式系统理论进阶：选举、多数派和租约.md)
* #### [分布式锁的解决方案](4.%20分布式/1.%20分布式理论/7.%20分布式锁的解决方案.md)
## 面试
### 计算机网络
* #### [HTTPS的加密机制](面试/计算机网络/1.%20HTTPS的加密机制.md)
### Spring
* #### [Spring Boot中的注解](面试/Spring/1.%20Spring%20Boot中的注解.md)
* #### [Spring Boot中的AOP及日志记录应用](面试/Spring/2.%20Spring%20Boot中的AOP及日志记录应用.md)
### Redis
* #### [Redis的IO多路复用](面试/Redis/1.%20Redis的IO多路复用.md)

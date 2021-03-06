---
title: 搭建微服务架构的四大核心（附方案分析）
date: 2017-06-09 19:32:18
categories: "开发"
tags:
	- 科技
	- 文章
	- 通信
	- 高峰
	- Facebook

---

# 服务的拆分 #

对于微服务架构项目，针对业务逻辑对服务进行合理的拆分是必不可少的重要工作之一，服务拆分是否合理直接影响到以后项目的易扩展性和易维护性。  


对于服务进行拆分应该从横向和纵向两个角度去做。

 *  **纵向**纵向上一般可以分为逻辑控制部分，业务服务接口，数据层操作，异步消息枢纽等。
 *  **横向** 横向拆分需要根据业务特点进行。拆分粒度太大，则微服务优势体现不明显，拆分粒度太小，各个服务耦合性可能太强，以后业务上的一点小调整可能需要涉及多个服务的改造。

另外服务的拆分也与业务的用户量有关，用户量小的项目一般不太适合使用微服务架构，用户量不大，则拆分粒度可相对大一点。

![搭建微服务架构的四大核心（附方案分析）][YJV3-AERI-QNNU.jpg]

--------------------

# 服务的远程调用    #

在微服务架构中往往存在着多个服务，服务之间如何高效的调用是微服务架构中的关键技术点。目前业内常用的方案就是基于**RPC**框架。常用的RPC框架有：Facebook开源的**thrift**、阿里开源的**dubbo**、**Hessian**等，不同的框架略有差异，根据笔者了解，thrift的优点在于可以跨语言调用，支持同步、异步等多种通信方式。dubbo的优点在于具有一套丰富完整的微服务方案，比如下面要提到的服务的管理。

在RPC框架的选型上，主要应以在通信方面的效率和性能为主，这也是RPC框架的一个核心点，最好是选择支持异步NIO的通信方式，至于其他功能，则可以通过一些分布式管理工具和中间件实现。对于分布式感兴趣的读者，可以点击文章末尾的关注，私信回复：**分布式** 给您看一篇常见高可用架构的分布式技术。  


![搭建微服务架构的四大核心（附方案分析）][7VZJ-ZYZ3-6VAN.jpg]

--------------------

# 服务的管理    #

在微服务架构项目中，往往存在者多个服务，每个服务有多个实例。由于业务有高峰和非高峰期，实例数目可能也是动态变化的。服务之间如何发现和调用的，服务失效之后又是如何移除的，同一个服务的配置应该怎样管理？常用的解决方案是使用zookeeper搭建一个服务管理中心，服务管理中心的主要功能是三个方面：服务的发布与订阅、服务的统一配置、服务的监控。关于如何基于zk搭建一个服务管理中心，将在明天的文章中进行介绍。  


--------------------

# 服务的跟踪    #

分布式服务往往有一个弊端，当一次请求出现问题之后，如何确定故障发生在哪一个服务和哪一个实例上。这往往是一个很头疼的问题，好几个服务，几十个实例中，如何快速定位？一般解决方案是在服务调用时传递三个信息：① 我是谁，以 “服务名+实例” 作为参数。② 我要调用谁，以下一个服务名+实例。③ 请求ID，根据业务来定，可以使userId或者session等。  


![搭建微服务架构的四大核心（附方案分析）][Y63Y-U3Q3-AQ7N.jpg]

感谢您阅读完原创本文，如果您对于**高可用与分布式架构**感兴趣，可以关注我，回复**分布式**，跟您看之前发布的一篇关于高可用方案的原创文章。  



[YJV3-AERI-QNNU.jpg]: /pro/os/crawler/YJV3-AERI-QNNU.jpg
[7VZJ-ZYZ3-6VAN.jpg]: /pro/os/crawler/7VZJ-ZYZ3-6VAN.jpg
[Y63Y-U3Q3-AQ7N.jpg]: /pro/os/crawler/Y63Y-U3Q3-AQ7N.jpg
 *  **原文作者：** IT技术百货
 *  **原文链接：** https://www.toutiao.com/item/6429270127702704642/
 *  **版权声明：** 本博客所有文章除特别声明外，均采用 [CC BY-NC-SA 4.0][] 许可协议。转载请注明出处。
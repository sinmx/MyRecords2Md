---
title: 机器学习如何入门？Kaggle CTO刚刚写了份详细的指南
date: 2017-03-27 11:06:40
categories: "开发"
tags:
	- 机器学习
	- Reddit
	- Quora
	- 人工智能
	- Kaggle

---

![机器学习如何入门？Kaggle CTO刚刚写了份详细的指南][Kaggle CTO]

> 李林 编译整理
> 
> 量子位 出品 | 公众号 QbitAI

上周，Ben Hamner很忙。

作为全球最大数据科学和机器学习竞赛平台Kaggle的联合创始人&CTO，他在Quora上参加了一场AMA，还参加了一场机器学习会议。会议我们最后再说，先说AMA：它是ask me anything的首字母缩写，美国reddit、Quora等社区经常邀请名人参加这种在线问答活动，比如说盖茨就每年都会在reddit上搞AMA。

**AMA中得票最高的答案是“研究机器学习和人工智能最好的资源是什么？”Hamner在答案中把机器学习的入门过程分成8步，写了一份详细的指南。量子位将要点编译如下：**

你很幸运，要开始研究机器学习和人工智能，现在是比任何时候都好的时机。这个领域近年来在快速发展，专业人士发布并改进着高质量的开源软件工具和库，每天都有新的线上公开课和博客文章出现。机器学习在各个领域每天贡献着数十亿美元的营收，带来了无与伦比的资源和大量工作机会。

这也意味着，你在刚接触这个领域时会有被淹没的感觉。下面是我的入门方法，如果你在研究过程中卡住了，去Kaggle上搜索一下，很可能有人遇到过和你类似的问题，如果没有，可以在我们的论坛上发帖提问，这是个获得指引的好办法。

# 1. 找一个你感兴趣的问题 #

从一个你想解决的问题入手，会更容易集中精力，也更有学习的动力，这种方法比照着一份长得吓人的散乱知识点清单来学习要好很多。和被动地阅读相比，解决问题也能驱使你深入到机器学习之中。

好的入门问题有以下几个标准：

 *  涉及你个人感兴趣的领域；
 *  有现成的数据适合用来解决这个问题，否则你需要花大把的时间来找数据；
 *  你能够在一台机器上流畅地处理这些数据，或者它的子集。

想不出来要解决的问题？上Kaggle嘛……Kaggle有个入门系列竞赛，提供了适用于新手的机器学习问题。推荐从泰坦尼克号乘客的生还概率预测（https://www.kaggle.com/c/titanic）开始。

# 2. 做一个快速、脏乱、黑客范儿的端到端解决方案 #

初学者很容易陷入一个实现细节之中，或者为错误的机器学习算法仔细调试，你需要避免这种错误。你的目标，是尽可能快地把端到端的基本解决方法做出来：读入数据、把它处理成适用于机器学习的格式、训练一个基本的模型、得出结果、评估它的性能。

# 3. 改进你的解决方案 #

现在，基本功能已经实现，发挥创造性的时候到了。你可以尝试对最初解决方案中的每个组件进行优化，然后测试修改带来的作用，搞清楚该在哪个部件上花时间。通常来说，获取更多的数据或者请洗数据之类的预处理步骤，比优化机器学习模型有着更高的投入产出比。

这些步骤可能需要你亲自上手处理数据，比如说通过检查特定的某一行、通过可视化方法来查看数据分布等方式，来更好地理解数据的结构和怪癖。

# 4. 写出来你的解决方案&分享 #

想要获得别人对你的解决方案的反馈，最好的方法就是写出来并分享。写出你的解决方案意味着你会以新的方式去看它，并加深理解，也能让别人理解你的工作并做出反馈、帮你学习进步。写作也有助于开始建立机器学习作品集，来展示你的能力，对找工作很有帮助。

我们以Kaggle数据集和Kaggle Kernels为例，它们分别可以用来分享数据和解决方案，从而获得反馈，看其他人如何对你的问题进行扩展。这也是丰富你的Kaggle资料的办法。

# 5. 在更多问题上重复1-4步 #

现在，你已经完成了一个自己喜欢的问题，接下来应该在不同领域的问题上多试几次。

你在入门的时候是不是用了表格式的数据？选一个要用到非结构化文本的问题，再试试解决图像相关的问题。

你是不是先解决了一个结构化的机器学习问题？很多有价值的创造性工作，一开始都有赖于从宽泛的商业或研究对象找到一个定义清晰的机器学习问题。

Kaggle竞赛和数据集为机器学习的两个方面：定义清晰的机器学习问题和原始数据来源提供了一个良好的起步点。

# 6. 认真地参加Kaggle竞赛 #

和上千人比赛着去解决同一个问题，尽力做到最好，是一个很好的学习机会，这能够驱使你在这个问题上不断迭代，找到解决问题的有效途径。

关于其他人是怎样解决问题排除bug的，针对某个竞赛的论坛上有着丰富的资源，kernels体现了其他人对数据的洞察，并且给你提供了一个轻易的上手途径，获胜者的博客文章则展示了什么样的方法效果最好。

Kaggle竞赛提供了和别人组队的机会，我们的社区成员有着不同的背景和技能，每个人都能从其他人身上学到东西。

# 7. 在专业领域应用机器学习 #

这让你在大部分时间中都能接触到机器学习，有助于自我提升。决定你想要成为什么样的角色、建立和这个角色相关的个人项目列表，是一个很好的开端。

如果你还没准备好应聘机器学习相关职位，也可以在你现在的岗位上开辟新项目、寻找提供咨询的机会、参与黑客马拉松和数据相关的社区服务机会、这些都能帮你在机器学习领域立足。专业领域的工作通常需要比较强的编程能力。

在专业领域应用机器学习，有这些价值的机会：

 *  将机器学习用于生产系统；
 *  专注于机器学习研究，将技术发展的最高水平向前推进；
 *  用机器学习进行探查、分析，来提升你的产品和商业决策。

# 8. 帮助别人研究机器学习 #

教人学习能帮你巩固对基础概念的掌握。教别人有很多不同的方法，你可以根据自己的风格选一个：

 *  写论文；
 *  做演讲；
 *  写博客文章和教程；
 *  在Kaggle、Quora等网站上回答问题；
 *  亲自指导；
 *  在Kaggle Kernels和GitHub上分享代码；
 *  讲课；
 *  写书。

--------------------

**One More Thing...**

这次AMA，其实Hamner最想谈的是Kaggle的未来，他在资料里列出了自己愿意回答的话题：

 *  Kaggle的未来
 *  开放数据
 *  Kaggle竞赛
 *  机器学习和AI
 *  数据科学工作流程
 *  产品和工程
 *  Kaggle为何加入Google

可惜Quora上的群众对Kaggle的未来似乎并不关心，反正竞赛照常举行，数据集照常提供，量子位也不知道这个未来该从何问起。

不过，吃瓜群众不关心Kaggle的未来也没关系。周五，Hamner还去纽约的机器学习大会MLConf上做了以《Kaggle的未来：我们从何处来，到何处去》的演讲，也就是我们开头说的那场会议。

在量子位（公众号：QbitAI）对话界面回复“**Kaggle**”，我们会把Hamner这次演讲的PPT发给你。

> **今天AI界还有哪些事值得关注**？
> 
> 在量子位（QbitAI）公众号会话界面回复“**今天**”，看我们全网搜罗的AI行业和研究动态。笔芯❤~
> 
> 另外，我们建了一个**机器学习入门群**，希望和大家互相帮助、共同进步。欢迎加量子位小助手的微信：**qbitbot**，介绍一下你自己，符合要求的，我们会拉你进群。


[Kaggle CTO]: /pro/os/crawler/QFZR-REFN-MUQR.jpg
 *  **原文作者：** 量子位
 *  **原文链接：** https://www.toutiao.com/item/6402009531299136002/
 *  **版权声明：** 本博客所有文章除特别声明外，均采用 [CC BY-NC-SA 4.0][] 许可协议。转载请注明出处。
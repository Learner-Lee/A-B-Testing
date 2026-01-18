# AB Testing

## \#1:

 **What exactly A/B testing is? Why you'll need it?**
 A/B测试究竟是什么？你为什么需要它？



### 1. 最经典的 AB Testing

![image-20260116141701085](assets/image-20260116141701085.png)











### 2. correlation VS. causation

相关性与因果关系



#### 穿有趣的衣服可以让人更开心

可能1：wearing funny shirts  ---->  being cheerful

可能2：being cheerful  ---->  wearing funny shirts

可能3：personality  ---->  being cheerful

​					                ---->  wearing funny shirts



#### Correlation does not imply causation

有关联性不代表有因果关系



**红色汽车出事故的几率更多**（红色让开车的人更激进）

**从大学毕业的学生可以更容易在职业生涯获得成功**（University education will，or，these people have higher ambition,  higher working capacity ,  just more money）





#### 那我们该如何确立因果关系呢

experiments！！

比如：抽10000个人，一半开红，一半开蓝，一年后再统计



#### 结论：有关联性不代表有因果关系，如果你只研究历史数据就很容易产生误区，所以我们需要做实验





## \#2:

 **When do you need to run an A/B test?**
 什么时候需要进行A/B测试？





### 1. 在互联网中进行AB测试

![image-20260116144538342](assets/image-20260116144538342.png)

![image-20260116144522395](assets/image-20260116144522395.png)

当团队做的一个视频使得看过视频的人购买力提高126%，但当将视频移到购买按钮旁边时，看过视频的人购买力反而下降18%

（这就是correlation VS. causation，只研究历史数据知道了其中的关系，但是不知道原因和结果是什么）





#### 然后我们就需要experiment！！

![image-20260116144936325](assets/image-20260116144936325.png)







### 2.What can you A/B test?

![image-20260116150449403](assets/image-20260116150449403.png)



**Version A 胜出**

support tickets 减少 28%

阅读文章和观看视频次数 增加 18%



**标题**

![image-20260116150846552](assets/image-20260116150846552.png)



**按钮颜色**

![image-20260116150854266](assets/image-20260116150854266.png)



**新特征**

![image-20260116150912416](assets/image-20260116150912416.png)



**价格**（high risk）

![image-20260116151003119](assets/image-20260116151003119.png)



**邮件标题**

![image-20260116151200571](assets/image-20260116151200571.png)



QR code

![image-20260116151313540](assets/image-20260116151313540.png)



facebook 发布一个AB测试，给一部分人看快乐的新闻，给一部分人看消极的新闻。看快乐的新闻的人评论会更加快乐，看消极的新闻的人评论会更加消极









### 3. 什么时候做 AB test



**Google AB test**

![image-20260116154016092](assets/image-20260116154016092.png)

像素级 AB test 只适合超级公司

（不应该所有都进行AB test, 也不能一点不做AB test）





#### ⭐使用AB test的规则

 **A/B testing is not conversion rate optimization it's research.**

A/B 测试并非转化率优化，而是一种研究方法。



"An experiment is only a failure if you fail to learn, even if metrics appear to go up — if you don't understand why the metrics changed you'll never be able to recreate or build on your success."

“一项实验只有在你未能从中学习时才算失败，即使指标看似上升了——如果你不明白指标变化的原因，你就永远无法复制或进一步巩固你的成功。”








#### Two key questions before starting an A/B Test

1.是否有足够的人来完成这个测试

2.A/B Test 真的是当前业务的最佳解决方案吗（ROI 投资回报率）





#### ⭐不需要A/B 测试的情况

**如果目标人数过少，不建议 A/B 测试**

![image-20260116160110165](assets/image-20260116160110165.png)





**如果你已经知道结果会是怎么样，不建议 A/B 测试**

如果你文档很烂，建议找个人优化文档，而不是A/B test



##### 如果什么都不会失去，就不需要A/B测试

非盈利不需要A/B测试



##### 如果人数过少，就不需要A/B测试



##### 如果回头客很多，就不需要A/B测试







#### ⭐需要A/B 测试的情况

**如果你想做出巨大改变，A/B测试一下**

比如：纯色的广告牌，夸张的标题，新加的动画效果



**如果这个产品已经成功了，但是你想做出巨大改变，A/B测试一下**



**价格较低的会让人冲动消费的产品，在尝试不同照片的时候，A/B测试一下**



**价格很高的产品，在尝试不同销售文案的时候，A/B测试一下**



**如果你想改变用户的初体验，A/B测试一下**



**如果你想尝试新东西，A/B测试一下**



**low-hanging-fruits 唾手可得的成果，A/B测试一下**







#### ⭐A/B test only when you need it(A/B test之前需要思考的问题)

1. Can i take the risk of not A/B testing this?
2. What will I learn from this A/B test?
3. Have we had a fight about this design/copy/feature in meetings before?











## \#3:

 **The statistics behind A/B testing.**
 A/B测试背后的统计学原理。

![image-20260117163201321](assets/image-20260117163201321.png)





### 判断结果是否是真实的或随机的

**A**

![image-20260117163532464](assets/image-20260117163532464.png)

**B**

![image-20260117163339441](assets/image-20260117163339441.png)

**C**

![image-20260117163748816](assets/image-20260117163748816.png)



统计显著性：91%

- 91% 的概率表明这些结果是真实的；
- 9% 的概率表明这些结果是偶然产生的。
- 发布你的获胜版本后，有 91% 的机会再次获得类似的结果。

------



#### A/B Test工具：Google Optimize

![image-20260117164120490](assets/image-20260117164120490.png)



#### 测置信区间的网站

![image-20260117164354420](assets/image-20260117164354420.png)







### A/A Test 测试 statistical significance

![image-20260117164621815](assets/image-20260117164621815.png)

version A 和 version B 完全一样



**A/A Test**

![image-20260117164816974](assets/image-20260117164816974.png)

测试结果是否随机







### 多高的Statistical Signigicance是好的level

![image-20260117165000135](assets/image-20260117165000135.png)



#### **先来看看实验**

![image-20260117170028586](assets/image-20260117170028586.png)

**返回AB测试**
![image-20260117170204379](assets/image-20260117170204379.png)

我们在A/B test中一定要避免假阳性



#### **返回Statistical Signigicance**

![image-20260117170450749](assets/image-20260117170450749.png)

![image-20260117170439354](assets/image-20260117170439354.png)

![image-20260117170426055](assets/image-20260117170426055.png)

**他们的虚假结果相差20倍**



如果风险承受能力**高**你可以相信90%，如果风险承受能力**底**你可以相信95% / 99%，学术界大部分接受95%



100% 不存在





### 样本量计算

- 目前转化率
- 想提升多少
- Statistical Signigicance

![image-20260117180445416](assets/image-20260117180445416.png)

**使用 Optimizely 样本量计算器**（**用户**）

![image-20260117181752677](assets/image-20260117181752677.png)

![image-20260117181914900](assets/image-20260117181914900.png)

![image-20260117181937509](assets/image-20260117181937509.png)

**时间**

![image-20260117182315201](assets/image-20260117182315201.png)





### A/B测试的四个步骤

1. Preparation（准备）
2. Implementation（实施）
3. Running an experiment（进行实验）
4. Evaluating the experiment（评估实验）

> Running reasearch before your experiments is 90% of the work and 90% of the success
>
> 实验前的调研工作占了90%的工作量，同时也决定了90%的胜利



#### A/B Testing 研究框架

![image-20260118143733804](assets/image-20260118143733804.png)



定性研究，定量研究（数据分析），头脑风暴，5秒测试，A/B Testing，最终版本发布。



##### **Qualitative Research 的常见方法是**：用户访谈，**可用性测试**，问卷调查。

它可以让你只是用很少的样本，就获得深入的理解









##### **Data Analysis**：

1. 分析方法：funnel analysis，segmenting，heatmapping correlation analysis and so on
2. Tools：Google Analytics，Mixpanel，Hotjar，Jupyter Notebook

**例子**

![image-20260118145422179](assets/image-20260118145422179.png)

**可用性测试显示：**
 用户不知道我们卖什么。

------

**数据分析显示：**

- 56% 的访客首先访问此页面
- 相比其他页面，跳失率高出 43%
- 相比行业基准，跳失率高出 36%
- 相比其他页面，用户互动减少了 65%
- ……



##### Brainstorm

给出好的修改Idea





##### 5 Second Testing

（当你有5 - 6个idea的时候，其中2-3个是非常不好的但自己发现不了，然后你就需要进行筛选）



**小测试**

![image-20260118151206759](assets/image-20260118151206759.png)

问题：这家公司在卖什么？







##### A/B Testing

![image-20260118151719027](assets/image-20260118151719027.png)













## \#4:

 **Executing a successful A/B test (step by step)**
 成功执行A/B测试（逐步指南）











## \#5:

 **A few smaller additions.**
 一些补充说明。











## \#6:

 **Summary. The right A/B testing mindset.**
 总结：正确的A/B测试思维模式。
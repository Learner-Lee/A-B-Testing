# AB Testing

## \#1: **What exactly A/B testing is? Why you'll need it?**


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





## \#2: **When do you need to run an A/B test?**

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











## \#3: **The statistics behind A/B testing.**

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









## \#4: **Executing a successful A/B test (step by step)**

成功执行A/B测试（逐步指南）





### A/B测试的四个步骤

1. Preparation（准备）
2. Implementation（实施）
3. Running an experiment（进行实验）
4. Evaluating the experiment（评估实验）

> Running reasearch before your experiments is 90% of the work and 90% of the success
>
> 实验前的调研工作占了90%的工作量，同时也决定了90%的胜利



### Preparation（准备）



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









### 当你有了一个好的Idea,并打算开始实施的时候，你还需要思考一件事情

⭐**如何衡量和评估你的A/B Testing是否成功**

- 你的成功指标应该在实验前就定义
- 你只能选择一个（坚持只看一个指标）

（因为我们需要避免观察者偏见）



![image-20260120210136375](assets/image-20260120210136375.png)

你有可能会很轻易的关注好的数据，而忽略坏的数据



#### 好的指标需要包含一下三个点

1. you have enough data points for it.
2. you seccess metric can't be logging metric （你的成功指标不能是滞后指标）
   1. ![image-20260120210726822](assets/image-20260120210726822.png)
   2. 有很多网站在注册30天之后才要交钱，这就不是一个好的指标，因为等待太久的时间
3. you seccess should be an important key metric in general for your online business（它是项目中的关键指标）
   1. ![image-20260120211115397](assets/image-20260120211115397.png)
   2. subscriptions number 太少了，所以应该看 click-through number







### 如何设置一个合适的假设

> “I'll do X and so i expect Y to happen”
>
> 如果我吧这个按钮改成红色，预计销售会提高50%

-  **The concept**
   - 概念：简要描述你想运行的A/B测试的概念，有哪些定性、定量研究去支持这个concept？
-  **The research result**
   - 你可以添加A/B测试相关的初步研究结果，发现了什么问题或机遇？哪些定性或定量数据点验证了这一点？你的定性研究发现了什么？数据分析的结果如何？
-  **what will you change?**
   - 你在你的在线业务的哪个部分做出哪些具体改变
-  **what results do you expect to see**
   - 你期待看到什么样的结果？
-  **How big of a sample size do you need? (how long your test will run?)**



#### example

![image-20260120214115860](assets/image-20260120214115860.png)

##### the concept

![image-20260120214211866](assets/image-20260120214211866.png)



##### The Research result

![image-20260120214319992](assets/image-20260120214319992.png)



##### **what will you change?**

![image-20260120214342547](assets/image-20260120214342547.png)



**what results do you expect to see**

![image-20260120214407840](assets/image-20260120214407840.png)



##### **How big of a sample size do you need? (how long your test will run?)**

![image-20260120214443190](assets/image-20260120214443190.png)

> 1. 它可以强迫你思考A/B Testing的方方面面
> 2. 它不会给你任何产生自我偏见的机会



### 一个好的A/B测试表格框架

![image-20260120214803239](assets/image-20260120214803239.png)





### Implementation（实施）

—— 市面上有很多点击式的A/B测试工具



#### 网站A/B测试

![image-20260120215814442](assets/image-20260120215814442.png)

- Google Optimize
  - 免费版就包含所有功能
  - 可以和其他的Google产品很好的协同合作
- Optimizely
  - 行业顶尖 
  - API connect
- VWO
  - 不太推荐





#### 新闻简报A/B测试

![image-20260120220048265](assets/image-20260120220048265.png)

![image-20260120220059518](assets/image-20260120220059518.png)

> 他们不是专门提供A/B testing 服务的，所以如果你算出了不同的数据，可以相信自己的





#### 广告A/B测试

![image-20260120220249643](assets/image-20260120220249643.png)

> 务必仔细检查统计显著性和结果的准确性





#### Tool DEMO

![image-20260121132834019](assets/image-20260121132834019.png)

> 自己实践
>
> 教程：https://www.youtube.com/watch?v=6R0PApm_bdQ&list=PLHS1p0ot3SVjQg0q1eEPrmOmPUY_AT1vB&index=23



#####  当你在点击开始按钮之前。。。。

1. Go through the "Can I start this experiment" checklist!
2. Ask one of your colleagues to review your A/B test!
3. Don't publish the A/B test the same day you set it up!



##### A/B 测试 it works with cookies

1. 情况一：使用常规浏览器进行访问，因为她的访问会带着cookie所以他不会发现A/B Test的迹象
2. 情况二：如果用户使用了隐身窗口或禁用cookie，服务器就会重新分发A/B Test的version，所以用户就有可能发现A/B Test的迹象。
3. 情况三：如果用户用不同的设备，也有可能发现A/B Test的迹象







#### Avoiding website Flickering in an A/B test

**正常情况**

![image-20260121170428967](assets/image-20260121170428967.png)



**但是如果 A/B 的 JS放在很后面，他可能会先刷新出Version A 然后再刷新出Version B，这个就叫闪烁。**

![image-20260121170657976](assets/image-20260121170657976.png)



**但是有时候，这个还是不够。因为当你将JS放在页面顶端的时候，它将减慢页面加载速度，这有可能会影响测试结果。所以你需要将JavaScript的代码片段设置为异步加载。**

![image-20260121171532560](assets/image-20260121171532560.png)



**但是这也会有个问题，当你改变较多时，或者用户的网络非常慢时，可能会导致JavaScript的代码片段加载很慢，造成“闪烁”问题。**

![image-20260121171745585](assets/image-20260121171745585.png)





**为了解决JavaScript的代码片段加载很慢，造成的“闪烁”问题，你可以额外加一个防闪烁的JS代码片段。这段代码如果检测到JavaScript的代码片段加载很慢时，会将该用户从实验中剔除，防止污染数据**

![image-20260121172135636](assets/image-20260121172135636.png)







#### 在A/B测试中常出现的问题

##### In an A/B test, you can only change one thing at a time.

(这是一个误区，你可以修改多个参数)

![image-20260121173426459](assets/image-20260121173426459.png)



**但是当你改变多个东西的时候是有风险的。**

> 比如说，有可能修改个标题可以提高转换率，但是修改颜色会降低，但你从结果看来只知道这样修改转换率会增加。（作者认为中小公司应该承担这种风险）

![image-20260121173800816](assets/image-20260121173800816.png)

> 大公司则不同，就算提高0.1%，也可以增加很多的利润

![image-20260121173906512](assets/image-20260121173906512.png)



- Big businesses should A/B test individual elements
- Small businesses should A/B test concepts.







##### Should I use multivariate testing?

> 理论上可行，但是只建议大公司

![image-20260121174329484](assets/image-20260121174329484.png)



> 你可以这样检测

![image-20260121174510827](assets/image-20260121174510827.png)



##### Can I run an A/B/C/D test?

> 理论上可行，但是只建议大公司

![image-20260121174618194](assets/image-20260121174618194.png)







##### Can I use a less usual, for example, a 30 - 70 audience split?

> 如果你很自信，你的新版本可以打败旧版本，可以这样做
>
> 这样既可以减少对原来业务的影响也可以得到不错的结果，然后如果确定新版本更好，可以从新改成50-50

![image-20260121174841525](assets/image-20260121174841525.png)





#### 企业都可能会犯的低级错误

1. 你应该随机分配Version A 和 Version B
   - ![image-20260121175704620](assets/image-20260121175704620.png)
2. Version A 和 Version B应该并行运行
   - 时间和季节可能影响A/B测试的结果
3. 你的用户不应该知道自己是实验的一部分
4. 响应迅速
   - 如果你Version B在手机打开中出问题了，这将会影响结果
5. 避免闪烁（同4）







### Running an experiment（进行实验）



#### How long should an A/B test run?

**决定持续时间的两件事**

1. statistical significance
2. rule of thumb: 2-5 weeks （最少2周【完整一周】，最多5周【在线业务需要快】）

![image-20260121181931957](assets/image-20260121181931957.png)







#### 不适合做A/B testing的时间段

1. Before/during holidays and special days
2. Don't release anything in friday (ON Fridays)你也不想毁了你的休息时间吧





#### 进行A/B测试的三个经典错误（root: emotion）

在你进行A/B测试的时候你会特别想你的版本成功，从而造成主观性的失败

- Stay strict and pragmatic（非常严格和务实）
- Best practice: Set a stopping rule before you start your A/B test!



1. **Never stop your A/B tests early on!**
   1. ![image-20260121191857274](assets/image-20260121191857274.png)
   2. ![image-20260121191917811](assets/image-20260121191917811.png)
   3. 只有保持在95% 或 99% 三天以上才停止实验
2. **Don't change anything in an ongoing A/B test!**
   - 要记住，A/B 测试是一个research，失败是常见的。我们可以从失败中吸收经验
   - 但如果你在A/B测试中做出了改变，将无法得到任何经验
   - ![image-20260121192432765](assets/image-20260121192432765.png)
3. **Don't check the interim result on a daily basis!**
   - Right after you start your experiment.
   - Once in every 3 or 4 days
   - After you've stopped your experiment.





### Evaluating the experiment（评估实验）

正常情况

![image-20260121192909125](assets/image-20260121192909125.png)



特殊情况：

- 嗯，好的，我们设置了99%的statistical significance，但是目前80%也行。
- 注册量是我们的主要成功指标，我们没能提高注册量，但是访问次数增加了，那就算Version B胜利了吧



![image-20260121193411916](assets/image-20260121193411916.png)

![image-20260121193518050](assets/image-20260121193518050.png)

![image-20260121193542295](assets/image-20260121193542295.png)







#### What to do when a test didn't perform the way you expected?（如果实验没达到预期怎么办）

![image-20260121195658729](assets/image-20260121195658729.png)



> 如果失败，尝试理解你的结果
>
> 你可以将测试结果，和定性研究和数据分析进行比较

![image-20260121195726872](assets/image-20260121195726872.png)





> 8个版本基本只能成功一个

![image-20260121195930316](assets/image-20260121195930316.png)







### 在结束前需要注意的两件事

- Documentation
- Follow-ups on your result



#### Documentation

![image-20260122130905597](assets/image-20260122130905597.png)

> 无论成功还是失败都需要写一份简短的总结

1. Your initial hypothesis and research result
2. Hard facts [确凿的事实] （conv% change and statistical signigicance level at the end of the test）
3. Additional thoughts —— conclusions, takeaways

》》》文档的长期目标是，创建公司内部知识库



#### Build an internal knowledge base

1. 它可以帮你回顾之前的实验【回忆起你做了什么以及为什么这样做 —— 你学要了什么，哪些不应该再进行A/B 测试】
2. 它可以帮助你的同事 【它可以让那些没参与的同时同样有收获，并从你所作的工作中学习】
3. 它可以帮助公司建立强大的 A/B testing culture





#### Follow-ups

> 可以看到长期的变化

**Example**

![image-20260122131213931](assets/image-20260122131213931.png)

在短期类的 subscribe 率 是提高了，但是长期来看，它的 cancel 率 高达100%【所以这是一个disaster】



但是，如果你想长期监控，需要自己写A/B testing程序，第三方软件基本上做不到这件事情。











## \#5: **A few smaller additions.**


一些补充说明。



### The limitations of A/B testing

![image-20260122131855680](assets/image-20260122131855680.png)

A/B 测试只适用于衡量短期效果

【在某些商业情况下，长远愿景比短期转化率的提高更为重要】



![image-20260122132210693](assets/image-20260122132210693.png)

每个测试只能揭示业务的一个部分，他们有可能有叠加部分，但是基本上不可能了解业务的全貌





### 有趣的悖论

![image-20260122133421762](assets/image-20260122133421762.png)

> There is a part of A/B testing that's more like an "art" than a science
>
> 【不同人会有不同的想法】



### Segmentation

different segmences may have different reaction for your different version of A/B test.

不同的用户群体，对不同版本的A/B测试可能有不同的反应



> 我们可以将移动用户和桌面用户分开

![image-20260122134330031](assets/image-20260122134330031.png)

**例如**

1. desktop vs. mobile vs. tablet
2. Asia vs. Europe vs. North-America vs. ...
3. different campaigns/sources









## \#6: **Summary. The right A/B testing mindset.**

总结：正确的A/B测试思维模式。

![image-20260122134730091](assets/image-20260122134730091.png)



- **mindset #1**：Correlation does not imply causation.
  - 分析历史数据只能显示相关性，只有实验才能发现因果关系
- **mindset #2**：A/B testing is not conversion rate optimization(转化率优化) it's research.
  - 你的首要目的是在实验中学习
- **mindset #3**：You should A/B test only when you need it —— but then, you should A/B test!
  - 有时候将精力投入市场或其他研究方法可以为公司带来更大价值
  - 但是如果需要进行A/B test但不进行，将会承担风险
- **mindset #4**：Statistics is important
  - 一定要注意statistical significance，不要gamble
- **mindset #5**：Preparation is 90% of the job and 90% of the success.
  - 一定要做好初步调研
- **mindset #6**：Practice makes perfect


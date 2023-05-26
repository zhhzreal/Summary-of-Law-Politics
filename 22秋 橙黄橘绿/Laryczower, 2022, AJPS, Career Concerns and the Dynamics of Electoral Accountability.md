# Career Concerns and the Dynamics of Electoral Accountability（AJPS）

### 本文作者

Matias Laryczower, Princeton University, Department of Politics, Professor. 

Gabriel Lopez-Moctezuma, California Institute of Technology, Assistant Professor. 

Adam Meirowitz, Yale University, Department of Political Science, Professor. 

<center><img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207120841078.png" alt="image-20221207120841078" style="zoom:47%;" /><img src="http://www.glmoctezuma.com/images/photo_me_caltech.jpg" alt="photo" style="zoom:4.9%;" /><img src="https://politicalscience.yale.edu/sites/default/files/styles/large/public/pictures/picture-3330-1662934894.jpg?itok=3rnWKD87" alt="亚当·迈罗维茨的画像" style="zoom:47%;" />

<center>本文作者

### 一句话总结

==选举问责制 Electoral Accountability==

美国参议员如何应对选举问责？

- 两方面的偏好：==职位 Office== 和 ==政策 Policy==

- 引入：==民意调查 Polls== ==政治立场 Ideology== 和 ==电视广告 Advertisement==三个参数来量化政治家对选举问责制的应对策略

### 文献综述

1. ##### 代议制民主的核心原则：选民通过选举规范政治家的行为

- 如果政治家偏离选民的偏好，选民可以通过投票让她下台
- 政治家的偏好：对职位的偏好（office），对政策的偏好（Policy）
	- 重视职位的政治家可能更愿意在政策上作出妥协，重视政策的政治家进行妥协的空间更小
	- 选举竞争的激烈程度、选民问责的强度也会影响政治家的行为
- 政治家的外部条件
	- 如果选民很容易被说服，那么政治家就没有必要在政策上作出妥协，而只需要试图影响选民（TV ads）
	- 如果选举问责很弱，政治家不容易收到惩罚，那么进行政策妥协的激励也比较弱

2. ##### 如何测量立法者对选民的回应？

- 立法者的投票行为
	- 假设：选民对立法者的投票行为知情、且做出一定的反应
	- 受到党派影响，许多选民对政治家的政策立场并没有明显的反应（Campbell et al., 1980）
- （Lim, 2013; Yoon, 2017）美国堪萨斯初审法院法官和州长的政策/职位偏好
	- 假设不同代理人是同质的
	- 本文：使用民调数据、政治家政策倾向、广告行为衡量政治家的偏好

### 研究设计

##### 数据：2000年-2014年，132次选举中美国各州共102位参议员

##### 过程

- 民调（Polls）数据公开 –> 政治家了解民调数据 –> 选择自己的政策倾向（Policy Position）/ 选择广告投入（Advertising）

- > Assumptions:
	>
	> 1. 对于政治家来说，购买电视广告是昂贵的
	> 1. 对于意识形态强烈的政治家，做出政策让步的成本更高
	> 1. Polls的结果不能完全预测，但跟最终选举的结果大致符合；Polls 的位置对政治家没有直接的影响，但是越临近选举，Polls的结果越重要
	> 1. 政治家取得职位会获得回报 $\omega$，如果是以巨大优势获得职位，还会获得额外的优势 $\alpha$（可能是0）

- 本文的实证检验

	- 1. 政策让步 Policy Concession 和选举结果 Electoral Gains 的边际替代率
		1. 电视广告和政策让步能够带来在民调/选举中的优势
		1. 把两者结合起来，在何种程度上政治家愿意做出让步迎合选民——选举问责制

##### 测量：

**Polls**：Polling Report, Real Clear politics, Pollster 数据

***==Pointlead==***：当月民调中“现任”和“挑战者”之间支持率的差异，加权平均值（权与受访者的数量成反比）

![image-20221207184420472](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207184420472.png)

**Policy** **Position**

>  i's positon in month t as her "ideal point"
>
> Bayesian Quadatic Normal Model

<img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207184649174.png" alt="image-20221207184649174" style="zoom:60%;" />

**Advertising**

GRPS: $广告总支出\over 广告总价格$

同时也计算了challengers的广告投入

<img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207185115593.png" alt="image-20221207185115593" style="zoom:50%;" />

**Additional** **Variables**

人口学变量+地区特征

##### 模型

##### ![image-20221207190156504](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207190156504.png)

t：距离选举的月份，T,…, 1

Pt：参议员观察到的民调结果

Xt：参议员选择的Policy Position

Et：参议员购买的广告数量

C(et)=$\gamma$et^2：购买电视广告的机会成本

u(xt, $\theta$)=-$\lambda$(Xt-$\theta$)^2：政治家进行政策让步的收益，$\theta$是政治家的“ideal point”，$\lambda$是意识形态的激烈程度

如果参议员赢得选举，获得$\omega$大于等于0；如果以较大优势赢得选举，获得额外奖励$\alpha$大于等于0

![image-20221207190921297](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207190921297.png)

$\theta$= -0.6 

​                                左：$\omega$=$\alpha$=0.2          中：$\omega=0.9$   $\alpha$=0        右：$\omega$=0  $\alpha$=0.9

控制变量：

<img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207192019248.png" alt="image-20221207192019248" style="zoom:50%;" />

![image-20221207192057634](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207192057634.png)

### 实证结果

##### 参议员对政策/职位的重视程度

![image-20221207192357415](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207192357415.png)

在选举前6个月，参议员愿意做出的政策让步

![image-20221207192600254](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207192600254.png)

广告的作用

![image-20221207192738325](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207192738325.png)

政策立场的变化

![image-20221207192834259](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207192834259.png)

把各州分为自由/保守，在意识形态最极端的州，采取极端的政策立场会获得回报；在意识形态比较温和的州，采取极端的政策立场会受到惩罚

电视广告的成本：参议员之间的异质性

![image-20221207193136560](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207193136560.png)

EAI：Electoral Accountability Index

![image-20221207200443191](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207200443191.png)

$\xi$ 当i的选举支持最大化时的政策位置

EAI=0 意味着政治家采取跟他意识形态一样的政策位置



选举优势和政治家的政策转变/广告行为

![image-20221207193248647](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207193248647.png)

竞争越激烈，政治家越倾向于进行政策调整/买广告

参议员的异质性

![image-20221207193545280](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207193545280.png)

女性/民主党/意识形态比较极端的参议员比较容易对选举问责进行回应

<img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207193715868.png" alt="image-20221207193715868" style="zoom: 67%;" />

反事实检验：把选举的回报扩大2/4倍

![image-20221207193847067](/Users/zhaohe/Library/Application Support/typora-user-images/image-20221207193847067.png)

回报增加会提高政治家的回应性

### 结论和讨论

立法者既有政策动机，也有任职动机

利用立场选择和广告行为量化参议员如何权衡政策让步和选举收益，以及这些因素如何影响他们对选举激励的响应



整体的结论好像不是特别难理解
## Intrinsic Social Incentives in State and Non-State Armed Groups(APSR)

### 本文作者

Michael J. Gilligan, Professor, Department of Politics, NYU. 

Prabin Khadka, AP, Department of Government, University of Essex. 

Cyrus Samii, Associate Professor, Department of Politics, NYU. 

![img](https://as.nyu.edu/content/dam/nyu-as/faculty/images/gilligan.jpg)

<center>本文第一作者
</center>

### abbr.

SAGs(State Armed Groups) 国家安全武装

NSAGs(Non-State Armed Groups) 非国家安全武装

### 一句话总结

实验

==非国家安全武装==和==国家安全武装==

由于 NSAGs 不能提供更加可靠的承诺，所以它们会选择对成员进行 Inculcation（政治教育？灌输？洗脑？），导致在 NSAGs 服役越久的士兵，越具有亲社会的倾向。



尼泊尔，科特迪瓦，伊拉克库尔德斯坦自治区（Peshmerga 自由斗士 / 佩什梅格）

### 文献综述

#### Inculcation

- 部队管理需要监控，但监控的成本是很高的/不可能的
	- 军事组织使用 inculcation 的手段，投入时间和金钱在军队内部培育忠诚和团队精神
- 内疚 guilt 和羞耻 shame
	- 两种都是一种社会惩罚
	- 羞耻 意味着不良行为==被发现==而受到惩罚
	- 内疚 与不良行为是否被观察到无关——节约监控的成本
	- 与此对应的还有 荣誉 honer 和骄傲 pride
- 什么是 inculcation？
	- 是指经过深思熟虑的、代价高昂的“训练”
		- 课程、材料、专门的时间
	- 不是服役过程中自然发生的，区别于社会纽带
	- “政治教育”
- 本文的假设：inculcation 是随着时间积累的，一个人服役的时间越长，接受的 inculcation 越多

#### NSAGs 的承诺问题

- 内战以后，国家将继续需要武装力量
	- 所以SAGs的士兵们有望重新入伍、晋升、领取养老金
	- 但NSAGs不能提供这样的承诺
		- 从历史的角度来看，许多NSAGs都不能信守承诺
- 所以，NSAGs更需要使用inculcation这种手段
	- 他们会在inculcation上付出更多成本
	- 提供即时的社会激励、弥补承诺的低可信度、规范成员的行为

#### Training

- NSAGs相对于SAGs会接受更多的inculcation
- 既有文献和本文访谈的佐证

### 研究设计

#### 假设提出

- 一个士兵在T年接受的inculcation：sT=$\sum_{t=1}^{T}l_t$
	- t 士兵的服役时间，如果接受了inculcation $l_t$ > 0, 否则为0

- H1: 对于两个服役了 T 年的士兵 i 和 j ，$T_i$ > $T_j$ , s$T_i$ $\geq$ s$T_j$. 
	- 服役时间越长，接受的inculcation越多
- H2: $S_{NSAG}$ $\geq$ $S_{SAG}$.
	- NSAG 接受的 inculcation 比 SAG 更多 

#### 实验设计

##### Game1: pay-it-forward

i j k 三人一组，每人被给予 E 资金

i 决定将多少资金交给 j，这个数额最终会被双倍给予 j

同时 i 被告知 k 也会把一定资金交给 i，这个数额同样会被双倍给予 i

![image-20230215152458756](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215152458756.png)

##### Game2: public-goods

12个人一组，每人被给予 E 资金

每个人决定要将多少资金交付给 group，同时他们会得到总额的 20%

（如果12个人每个人拿出10块，他们最终会每人得到24块）

![image-20230215152512742](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215152512742.png)

- 两个实验的社会最优策略都是捐出自己所有的资金，但个人的物质动机要求他们贡献 0
- S(s$T_i$, $c_i$) social utility function
	- S = $\sigma$s$T_i$ ln($c_i$)
	- maximizing this utility
		- Game1 $c_i$ = $\sigma$s$T_i$ - 1
		- Game2 $c_i$ = 1.25$\sigma$s$T_i$ - 1
	- 在回归分析里，把两个游戏的结果合在了一起
		- $\beta$ = 2.25$\sigma$s
		- <img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215153125868.png" alt="image-20230215153125868" style="zoom:50%;" />

### 实证结果

#### 尼泊尔

- 背景介绍
	- PLA 毛主义政党
	- 1990年代从共产主义派系中分离出来，1996年开始“人民战争”
	- 2006年11月与当局签署全面和平协议，结束战争，转变为一个合法的政党

- 2012.7-2013.3 17个地区204个样本量
- ![image-20230215160829531](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215160829531.png)
- ![image-20230215160852293](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215160852293.png)
	- 服役时间越长，实验中的利他行为越多
	- selection bias？
	- ![image-20230215161222695](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215161222695.png)
- 问题
	- 毛主义政党主张平等的价值观：结论有普遍性吗？依靠农村进行斗争
	- 无法对尼泊尔的SAGs进行研究
	- 小样本
	- 解决方法：其他地区

#### 科特迪瓦

- 背景介绍
	- 2002年爆发了基督徒和穆斯林之间的冲突
	- 基督徒的领导人 Gbagbo
	- 支持Gbagbo的两支力量：陆军（SAG） 民兵（NSAG）
- 5次实验
- ![i](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215161755439.png)
- ![image-20230215162209040](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215162209040.png)
	- 服役时间越长，亲社会行为越明显
	- 在SAG服役的士兵，亲社会行为下降
- ![image-20230215162123295](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215162123295.png)
	- 在第一次敌对期（2005-2008）死亡率上升

#### Peshmerga

- 背景介绍
	- 伊拉克库尔德斯坦自治区的武装力量
	- 2003年美国入侵伊拉克以后，Peshmerga 从一个NSAG 转变为了 SAG
	- 2014年1月，伊斯兰国入侵该地区，Peshmerga 队伍的组成 又 发生了变化
	- 所以产生了一个自然的分组：2003年以前入伍，2003-2012年入伍，2013年以后入伍
- 17次实验，192个样本量
- ![image-20230215162836600](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215162836600.png)
- ![image-20230215162859924](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215162859924.png)
	- 2003年以前入伍的士兵，服役时间越长亲社会行为越多
	- 2003-2013年入伍的士兵，服役时间越长亲社会行为越少
	- 2013年以后入伍的士兵，服役时间越长亲社会行为越多
	- ！
- ![image-20230215163010791](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215163010791.png)
- ![image-20230215163043473](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215163043473.png)
	- 2003年以后，战争的烈度下降，基本符合该地区的历史

#### 对结果的质疑

- 民兵组织意识形态的影响？
	- 尼泊尔 是毛主义政党，科特迪瓦 民兵的意识形态是排外的，但在实验中都表现出了同样的行为
- 跟民众的接触？
	- 尼泊尔 跟农民有密切的接触，科特迪瓦 的民兵虐待平民
- 外部有效性？三个地方都表现了同样的趋势
- 小样本？三个地区

- inculcation 在发挥作用？随着战争的进行，更光明的前景提高了民兵的心理预期？
	- 尼泊尔 可能是这样的
	- 但在 科特迪瓦，民兵组织的情况是不断恶化的
- self- selection rather than inculcation？
	- 如果有一些人天生就是热爱为人民服务的，那么他们更亲社会的原因不是inculcation，而是服务人民更久
	- 毛主义政党 同样在农民之间进行政治教育，但接受政治教育时间更长的农民并没有同样地表现出亲社会的倾向
		- <img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20230215164922357.png" alt="image-20230215164922357" style="zoom:50%;" />
- SAG和NSAG本身没有区别，只是民兵更容易被洗脑？Peshmerga的例子

### 结论和未尽的问题

NSAGs没有办法提供可置信的承诺，所以它们选择将更多的成本投入到 inculcation中，改变组织成员的偏好

这种行为提高了民兵的亲社会性



看起来像是把三个有selection bias的案例放在一起

案例选择

挺好玩的


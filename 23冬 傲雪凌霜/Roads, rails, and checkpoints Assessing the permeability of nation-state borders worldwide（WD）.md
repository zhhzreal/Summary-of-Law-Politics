# Roads, rails, and checkpoints: Assessing the permeability of nation-state borders worldwide（WD）

### 数据和研究设计

### 数据

OSM：开源的地图协作平台

世界粮食计划署的全球边境过境点

B' Tselem, 2021 补充了 以色列-巴基斯坦 的边境线



GIS数据库：利用PostgreSQL/PostGIS衡量穿过边境线的交通设施

#### 定义 infrastructure-based border permeability

<img src="/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124124349885.png" alt="image-20230124124349885" style="zoom:50%;" />

A：一段100km长的边境线

B：边境上有一条公路通过（黑色实线）——渗透率比较低

C：边境线上有很多公路通过——渗透率比较高

D：边境线上有公路和铁路（黑色虚线）通过——渗透率比较高

E：公路上有检查站——降低渗透率

F：几乎每条公路上都有检查站——渗透率进一步降低

#### Quantitative Border Permeability Index (BPI)

![image-20230124124935403](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124124935403.png)

L：边界线的总长度

I：所有穿过边界线的铁路、公路、道路总数

C：检查站的数量

e：检查站的控制程度/执法的严格程度 [0, 1]

- 0——检查站实际上没有使用
- 1——检查站实际上拒绝一切人/物通过
- 没有具体的经验信息，用e作为参数显示边界渗透性的变化

s：normalize 使BPI的取值范围在[0, 1]之间

### 问题：I 的衡量？

![image-20230124125522745](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124125522745.png)

交通设施的多样性的吞吐量的差异：公路、铁路、自行车道、小路……

$w_i$是赋予该种交通设施的权重，$i_n$是交通设施的类型（n=38）

- 根据OSM赋予交通设施权重，且同时考虑加权和不加权的结果
- 人工检查（25.4%，人工只区分公路或铁路、渡轮）
- 无法区分“特殊道路类型”和“自行车道”——赋予相同的权重
- 一个检查站对应多条道路——取平均值
- 聚类
	- 如果一个城镇刚好位于边境线上，可能有大量道路穿过它，但沿着边境线的其他地方的交通设施可能很少——500米范围内发现多个跨境交通基础设施时，只计算一个 使用DBSCAN完成
	- 检查站 250米
- 人工检查
	- 终点接近边境的道路被误报？遗漏？渡轮？
	- 3 human coders，several months, 6996个识别错误被删除，7615个遗漏被添加
	- 覆盖312个陆地边界，30045个可用跨境交通基础设施，2939个检查站

形成了==BPI==和==non-weighted BPI==

#### 回归模型

分析单位：国家对，双向A-B，B-A，因此样本量x2（BPI没有方向性，但是一些自变量是有方向的）

因变量：BPI

自变量：

- 经济：
	- GNI 人均国民总收入
	- 两国绝对GNI 差异
- 政治：
	- 两国共同加入的政府间组织数量；
	- 两个国家的平均民主得分（经济学人, 2018）；
	- 1945-2020年右翼政府首脑任职年数
- 流动性：GHS
	- 人类居住密度
	- 人类定居点密度
	- GMP 全球跨国流动性数据
	- GMP 各国互相收取的旅游签证费用
- 文化：
	- CEPII 共同口语(Melitz & Tubal, 2014)，宗教临近性
- 控制：
	- 边界长度

回归模型: OLS with dyad-adjusted standard errors

### 实证结果

#### 描述性统计

![image-20230124182834645](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124182834645.png)

欧洲最高，非洲其次；是否加权对结果的影响不大

![image-20230124182911780](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124182911780.png)

为什么加不加权影响不大？除了北美以外，平均的交通设施全种类似

为什么北美不一样？汽车文化，缺乏行人和自行车道，街道更宽；

总的来说，世界各地的交通基础设施组成非常类似

![image-20230124183050360](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124183050360.png)

检查站的数量：中东、北美、欧洲更高，对边界渗透率有明显的负面影响

欧洲的边境要更加开放

![image-20230124183237921](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124183237921.png)

西欧、中欧、东欧、东南亚、东非、西非

![image-20230124190339171](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124190339171.png)

B：BPI的分布 Andorra-Spain border

- 前20名几乎都来自欧洲，通常是小国，西班牙-安道尔，斯洛文尼亚-奥地利，卢森堡-法国
- 马拉维-赞比亚，马拉维-莫桑比克来自非洲；案例研究显示这些地区的居民更倾向于认为“跨境是正常的”

C：取对数以后，看起来是正态

#### 回归结果

![image-20230124191506127](/Users/zhaohe/Library/Application Support/typora-user-images/image-20230124191506127.png)

Economics 和 Mobility 最重要

也就是经济发展水平和人口密度

Politics在 Full model 中不显著



经济发展水平的U形关系：经济最发达的地区和经济最不发达的地区渗透率比较高，中间水平的渗透率不高



### 结论和未尽的问题

理论上新的切入点

U型关系：发达国家更依赖商品贸易流动，落后国家/殖民国家的控制力更小

公开数据：https://doi.org/10.5281/zenodo.7457746



好伟大的工作量

方法上的讨论？

- 回归模型是线性的，结论是U型的
- 好像整个回归都不是特别有必要
- e的测量？
	- 没有找到合适的代理变量/测量
	- 但按照作者的理论，发达国家和欠发达国家的边界控制能力应当是不一样的






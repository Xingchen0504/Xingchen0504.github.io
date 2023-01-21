# planning
## paper list
## paper rank
### 会议
CV三巨头 CVPR,ECCV,ICCV；其他AAAI，ICML，NIPS <br />
机器人 ICRA：IEEE International Conference on Robotics and Automation <br />
IROS：IEEE/RSJ International Conference on Intelligent Robots and Systems <br />
ROBIO：IEEE International Conference on Robotics and Biomimetics <br />
### 期刊
cas
IEEE TIE中文工业电子，是大同行都比较认可的 <br />
IEEE ITS，方向偏交通 <br />
IEEE TVT发文量比较大 <br />
VSD 动力学顶刊 <br />
IEEE TIV, IEEE TTE属于后起之秀，发文量都不大，都有国内 <br />
## Learning materials
[apollo](https://apollo.baidu.com/) <br />
[大疆司康哥](https://scholar.google.com.hk/citations?hl=zh-CN&user=Yv4WunEAAAAJ) <br />
[实践](https://github.com/zhm-real/PathPlanning) <br />
> 包含可视化 <br />

## company tech
## 基础
### 动力学模型
### 计算几何
--------------------------------------------------
# MDP
expect max 最大期望算法 <br />
决策节点 当前所在的节点 可以进行决策 <br />
机会节点 决策者无法控制的情况 根据概率转移 <br />
选择每个决策的加权效用，采取平均效用最大的决策 <br />
# POMDP <br />
从某个先验信念状态开始，根据agent所在的信念状态，基于某个决议过程来确定选择某个动作执行，执行动作后受到观察值，使用滤波算法更新执念状态<br />
POMDP 是一种建模方式，考虑到当前状态的不确定性，即为信念状态，S是状态集合，A是决策/动作集合，P是s和a到新s的转移概率，R是状态s动作a的奖励，Π是观察集合，O是状态s获得o观测的概率。<br />
相当于用o去推测s

-------------------------------------------------
# 博弈论
## 静态博弈和动态博弈
静态博弈就是博弈双方做出的行动是同时的，博弈双方在作出行动的时候，其作出行动的依据并不是有对方之前的行动，其作出的行动完全是由于基于自己目前掌握的信息。或者做出行动的时候，并不知道对方的行动，静态博弈，大多数是一次性的博弈。比如石头剪刀布<br />
动态博弈是指动态博弈双方在做出行动的时候，依据对方之前做出的行动。至少在作出行动的时候，双方不是同时行动的。比如<font color="#dd0000">下棋，辩论</font>等<br />
静态博弈不存在完美不完美的分类 <br />
### 完全信息静态博弈
每个参与人对其他所有参与人的特征、策略空间及支付函数有准确的认识 <br />
### 不完全信息静态博弈
每个参与人对其他所有参与人的特征、策略空间及支付函数并没有准确的认识。<br />
### 完美信息
在博弈论中特指参与人完全了解博弈历史的一种信息结构。如果参与人在采取行动时并不完全了解博弈的历史，即并不完全了解其他参与人在他决策之前的所有行动，则这样的信息结构称为“不完美信息”。<br />
### 完全信息
是指每一参与者都拥有所有其他参与者的特征、策略集及得益函数等方面的准确信息的博弈。<br />
### 完全且完美信息动态博弈
完全且完美信息动态博弈简称动态博弈，也称为多阶段博弈、序列博弈或扩展形博弈。完全且完美信息动态博弈的特征是博弈方依次选择行为，后选择行为者是在看到先选择行为者的选择后再选择，博弈方相互了解得益情况。如斯塔克伯格模型<br />
### 不完全但完美信息动态博弈
完美/精炼贝叶斯均衡 <br />
## 零和博弈和非零和博弈

零和博弈属非合作博弈，一方获益意味着另一方损失 <br />
非零和博弈属合作博弈，可能共赢或者共输，综合大于零时为正和博弈，小于零为负和博弈 <br />
## 纳什均衡
在一个博弈过程中，无论对方的策略选择如何，当事人一方都会选择某个确定的策略，则该策略被称作支配性策略。如果<font color="#dd0000">任意一位参与者在其他所有参与者的策略确定的情况下</font>，其选择的策略是最优的，那么这个组合就被定义为纳什均衡。确定的是固定策略时，为纯策略纳什均衡，非固定策略时为混合策略纳什均衡，纯策略是混合策略的特例。 <br />
NE(完全） ————————SPE（完全且完美） <br />
BNE（不完全）————————PBE（不完全但完美） <br />
NE（纳什均衡）<SPE（子博弈完美均衡）<BNE（贝叶斯纳什均衡）<PBE（完美/精炼贝叶斯均衡） <br />
NE（纳什均衡）信息完全 静态博弈 <br />
BNE（贝叶斯纳什均衡） 不完全信息 静态博弈 <br />
SPE（子博弈完美均衡）完全完美信息的动态博弈 <br />
PBE（完美/精炼贝叶斯均衡） <br />
NE和BNE都是静态博弈的均衡，SPE与PBE都是动态博弈的均衡） <br />

--------------------------------------------------

# c++
## code style
## 多线程
## 并发

--------------------------------------------------
# 设计模式
--------------------------------------------------
# 其他
--------------------------------------------------
# 设计模式
--------------------------------------------------
--the end--

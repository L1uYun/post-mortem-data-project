# 贡献者

姓名或网名:高铭辰
(可选) 学号:202208060115

## 0 偶数组背景

对于历史，有很多历史并不客观，是经过了后人的改写才成为我们今天看到的历史，而且对于历史，能记录并传承下来的很少很少，有人就想要构建一个平台，让用户去这个平台上传自己的日记之类的内容，并在用户死亡后很多年后进行分析，这样就可以构建出人类更为全面的历史。


## 1 你认为可以研究的科学问题

Q1:
**“多主体、跨代际隐私”的新隐私模型**
日记里几乎必然包含其他人（配偶、子女、同事）的信息：
“今天我跟 X 大吵了一架，他患有抑郁症，我很害怕他做傻事……”
几十年后公开，会暴露这些还活着、或者后代的隐私。这是现有隐私模型（单主体差分隐私）里很少被认真处理的问题。

现有的隐私模型通常假设一个数据点 = 一个个体，而这里：
一个日记条目 = 一个事件，涉及多方；
这些人的“死亡时间 / 隐私偏好”可能不同；
如何定义一个多主体、跨时间的隐私保证？比如：
只要事件中有任意一位相关人还在世或不愿公开，
就必须对日记内容做某种形式的模糊。

## 2 你找到的相关工作

### 互依隐私 / 多主体隐私（Interdependent Privacy）
+  Interdependent Privacy: Let Me Share Your Data
   Biczók & Chia, Financial Cryptography 2013 
   经典的“互依隐私”起点文之一，形式化讨论：一个用户在 OSN 里的分享行为如何影响他人的隐私。
+ Modeling Interdependent Privacy Threats
   Liu & Biczók, arXiv 2025 
   更近期的工作，从更系统的角度建模 interdependent privacy 的威胁，强调数据共享生态中多方依赖。
   有比较新的威胁模型和形式化框架，你可以借鉴其“威胁空间/攻击面”的组织方式。

### 多方 / 群体差分隐私（Multi-party / Group DP）
+ Secure Multi-party Differential Privacy
   Kairouz, Oh, Viswanath, NeurIPS 2015 
   经典工作：多方持有数据，交互计算函数，同时保证各方差分隐私。
   你可以关注它的形式化 DP 定义、多方交互协议设计，思考如何把“party = 用户”变成“party = 日记里涉及的主体集”。
+ TPMDP: Threshold Personalized Multi-party Differential Privacy via Optimal Gaussian Mechanism
   Liu et al., arXiv 2023 
   提出“门限个性化多方差分隐私”：每个参与者有不同的隐私预算，还考虑了有限数量的共谋对手。
   对你来说，它的价值在于：不同主体不同隐私需求的建模方法，可以迁移到“不同人物不同生前/死后公开策略”。

### 死后隐私 / 数字遗产（Post-mortem Privacy & Digital Legacy）
+ Post-mortem privacy and informational self-determination
   Buitelaar, Ethics and Information Technology 2017 
   系统讨论了“死后隐私”的概念，把它与信息自决权联系起来。
   你可以从中抽取：死后隐私的定义；与在世隐私权的相似与不同点；
   这为你设计“跨代隐私策略”提供理论基础。

## 3 你想到的英文论文标题 (建议 3 到 5 个)

Title 1:**Intergenerational Multi-Subject Privacy: A Formal Framework for Posthumous Personal Data Release**
+ “Intergenerational Multi-Subject Privacy” → 一眼看出是 privacy 新概念 / 新定义。

+ “A Formal Framework” → 明确告诉 reviewer：这是 formal model + 定义 + 证明 型的贡献，不是纯 survey/讨论。

+ “Posthumous Personal Data Release” → 把你的动机（日记、死后数据）点出来，但放在标题后半句，不压过技术关键词。

Title 2:**The Living, the Dead, and Their Events: Intergenerational Multi-Subject Privacy for Posthumous Data Release**
+ 前半句有点 catchy，但仍然技术相关（the Living, the Dead, and Their Events）；
+ “Intergenerational Multi-Subject Privacy” 作为 subtitle 中心结构；
+ “Posthumous Data Release” 明确主题。



## 4 你认为可能的科学价值和创新点

提出并实现一个面向“跨代、事件级、多主体数据”的形式化隐私框架，支持死前/死后、不同主体间隐私偏好的统一建模和可证明保护。


## 5 你个人已经做了哪些工作

如上
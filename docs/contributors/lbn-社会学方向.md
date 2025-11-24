# 贡献者

姓名或网名: 罗贝妮
学号:202202010212

## 1 可以研究的科学问题

Q1:**“人机混合”写作下的历史真实性界定**

**基于论文:** *'It was 80% me, 20% AI': Seeking Authenticity...* (CSCW 2025)
**科学问题：** 现在的用户普遍使用大模型辅助写作（Co-writing）。Hwang 等人的研究表明，用户会主观地认为“80% 是我，20% 是 AI”。但对于历史归档来说，那 20% 的 AI 生成内容往往掩盖了人类2独特的语言特征。未来的历史学家如何从档案中剥离这“20% 的 AI 杂质”，还原纯粹的人类原声？如果无法区分，我们记录的将是“被 AI 修正过的文明”。

Q2:**递归数据训练导致的历史“模型坍塌”** 

**基于论文:** *AI models collapse when trained on recursively generated data* (Nature 2024/2025)
**科学问题：** Shumailov 等人在 *Nature* 上证明，如果模型反复在 AI 生成的数据上训练，会丢失分布的“长尾 (Tails)”——即那些罕见但珍贵的人类细节。本项目的目标是构建长达百年的历史模型，如果输入的数据中混杂了大量 AI 生成内容（Synthetic Data），模型最终会“坍塌”，导致构建出的历史变得平庸、单一，失去了人类社会的多样性。我们如何设计一种“长尾保护机制”？

Q3:**生成式 AI 时代的“死后数据管理原则”** 

**基于论文:** *Towards Post-mortem Data Management Principles for Generative AI* (arXiv Sep 2025)
**科学问题：** 传统的数字遗产管理只关注“存储与访问”，但在 2025 年，Van Kempen 等人提出核心风险在于“生成 (Generative)”——即利用死者数据训练新 AI 的权利。我们需要确立什么样的伦理原则，既能利用死者数据构建“人民历史”，又能防止死者的人格被算法随意“生成”和篡改？

## 2 找到的相关工作

**论文题目:** **'It was 80% me, 20% AI': Seeking Authenticity in Co-Writing with Large Language Models**

**发表:** *Proceedings of the ACM on Human-Computer Interaction (CSCW)*, May 2025
**和本方向的关系:** 该研究深入探讨了用户在人机协作中对“真实性 (Authenticity)”的感知。它揭示了“前台表演”现在变成了“人机合谋”。这为我们清洗历史数据提供了关键的社会学指标——必须标注出数据中的“AI 成分占比”，否则历史档案将失去信度。

**论文题目:** **AI models collapse when trained on recursively generated data**

**发表:** *Nature*, Vol 631 (2024), Updated March 2025
**和本方向的关系:** 这是一篇警告性的奠基之作。它证明了“递归训练 (Recursive Training)”会导致模型不可逆的退化。对于本项目而言，这意味着如果我们不加筛选地全量收集互联网数据（其中包含大量 AI 生成文本），我们的“历史大模型”将在几代迭代后彻底崩溃，变成只会说套话的机器。

**论文题目:** **Towards Post-mortem Data Management Principles for Generative AI**

**发表:** *arXiv:2509.07375*, Sep 2025
**和本方向的关系:** 该论文专门针对“生成式 AI”背景下的死者数据权利提出了管理原则。它填补了本项目在伦理设计上的空白：即如何定义死后数据的“生成权”。这直接关系到项目是否合法合规，是否尊重了“数字遗骸”的所有者。

## 3 英文论文标题

Title 1:
**The "Human Label": Separating Real Human Writing from AI-Assisted Text in History Archives**

Title 2:
**Saving the "Rare Stories": Protecting Human Diversity from AI Data Pollution and Model Collapse**

Title 3:
The Right Not to be Resurrected: Ethical Rules for Recreating Dead People with AI

## 4 你认为可能的科学价值和创新点

- **现有工作缺了什么**:
大多数历史归档项目只关注数据的“保存（Preservation）”，默认数据是**“纯人类产生 (Human-generated)”** 且 “分布稳定 **(Stable Distribution)**” 的。
- **我们想补什么空缺**:
基于上述三篇论文，指出 2025 年面临的两大新危机：“混合写作”导致的真实性稀释，以及“合成数据”导致的模型坍塌。
- **相比已有工作有什么新的视角或方法**:
    1. **引入“AI 成分标注”**：建议为每一条历史数据打上“80% me / 20% AI”的标签（灵感来自 Paper 1）。
    2. **反坍塌采样策略**：在训练历史模型时，故意对“长尾数据”进行过采样（Over-sampling），以对抗 Nature 论文中提到的分布消失问题（灵感来自 Paper 2）。

## 5 个人做的工作

- **前沿资料收集**: 重点调研了 2024-2025 年关于 Generative AI (生成式 AI) 与社会学交叉领域的最新进展
- **问题定位**: 结合 Nature 关于 "Model Collapse" 的理论，思考了该现象在本作业中的体现。我认为本项目最大的难点不仅仅是存储，而是如何防止历史模型因为摄入过多 AI 生成数据而“退化”。
- **概念学习**: 学习了 CSCW 2025 论文中关于“人机协作写作”的定义，了解了目前学术界对于“数字内容真实性”是如何量化的，为小组后续讨论提供了理论依据。

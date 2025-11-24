**贡献者**

姓名：陈仕茂

学号：202204060306

**1 你认为可以研究的科学问题**

Q1：如何在隐私数据中重建历史构象，得到人类行为模式、兴趣、社会身份随时间演化的轨迹，同时确保无法对个体进行逆向重识别？

Q2：如何阻断隐私在多代模型之间的跨代遗传，使模型体系不形成难以清除的长期隐私记忆？

**2 你找到的相关工作**

- **Quantifying Temporal Privacy Leakage in Continuous Event Data** — M. Rafiei et al., 2022.

   关键词：temporal leakage, continuous release, privacy metrics.
  
   关联：扩展并实证化“时间相关导致的隐私泄露”概念，可直接用于衡量长期数字痕迹在历史重构中的风险。

- **Bistochastically Private Release of Longitudinal Data** — N. Ruiz et al., 2025.

   关键词：longitudinal data, privacy-preserving release, longitudinal DP.
  
   关联：针对纵向（decade-scale）数据的差分隐私扩展/方法，直接关系到如何在保留时间结构同时保护隐私，从而支持 Q1 中“在保证不可逆识别下重构群体轨迹”的技术路径。

- **Machine Unlearning: A Comprehensive Survey** — W. Wang et al., 2024.

   关键词：unlearning survey, deletion methods, empirical evaluation.
  
   关联：综述机器忘却领域的现状与局限，指出在多代模型/蒸馏场景下隐私残留的若干未解问题。

- **Machine Unlearning of Pre-trained Large Language Models** — J. Yao et al., 2024.

   关键词：LLM unlearning, right-to-be-forgotten, pretraining.
  
   关联：研究如何对预训练大模型执行删除操作——Q2 关切模型谱系（pretrain → downstream → distillation）中隐私如何被继承/残留，该论文直接触及大型模型场景。

- **A Privacy-Preserving Knowledge Distillation Framework (Swing Distillation)** — J. Li et al., 2022.

   关键词：knowledge distillation, privacy-preserving distillation, teacher→student leakage.
  
   关联：研究如何在知识蒸馏过程中尽量阻止教师模型的私有信息流入学生模型，与 Q2 的“跨代遗传”思路相关。

**3 你想到的英文论文标题**

**Title 1：Unlinkable Historical Reconstruction: Learning Long-Term Human Behavioral Trajectories Without Identity Reassembly**

核心想法：提出一种框架，可在不恢复个体身份的前提下，从长期隐私数据中学习群体级历史构象与行为演化结构。

**Title 2：Temporal De-Configurability: Breaking Individual Traceability in Longitudinal Behavioral Modeling**

核心想法：构建时间层面的去构象化机制，使长期隐私数据无法被跨期关联，从而阻断身份重组攻击。

**Title 3：Privacy Lineage Breakers: A Training-Time Framework to Stop Privacy Propagation Across Model Generations**

核心想法：提出训练阶段的结构性机制，使得隐私表征无法沿着模型蒸馏或权重继承链持续传播。

**4 你认为可能的科学价值和创新点**

**4.1现有工作缺了什么？**

**4.1.1 缺乏可建立长期人类行为结构的隐私保护建模框架**

现有差分隐私、k-anonymity、synthetic data 等方法通常只关注一次发布或局部分析，无法支持：

- 数十年时间跨度
- 行为模式与兴趣的宏观演化规律
- 隐私保护的结构化信息学习

本研究填补“**长期、跨期、多模态人类行为结构**”在隐私保护条件下重建的空白。

**4.1.2. 解决时间维度隐私累积与跨期链式攻击问题**

长期隐私收集导致“时间关联性”极强，这可能建立起：

- 兴趣发展轨迹
- 社会身份迁移链条
- 行为驱动模型

我们首次系统研究“**历史构象下的隐私可逆性**”。

**4.1.3. 弥补“遗忘 vs 权重继承”的机制缺口**

现有机器machine unlearning只关注**单模型**，没有研究：

- A → B → C 多代模型
- 前代模型遗留隐私是否被继承
- 被蒸馏/迁移到子代中的隐私如何检测、消除

本研究补齐这一缺失的理论基础。

**4.2.创新点**

**4.2.1. 提出“历史构象重建”的隐私建模任务（全新任务定义）**

这是尚无定义的研究任务：在保护个体不可逆识别的同时，重建长期群体行为演化结构。

**4.2.2. 提出“Temporal De-Configurability”机制**

创新定义一种新机制，使同一人的跨期数据**不可对齐、不可拼接、不可关联**。

**4.2.3. 使用结构级别匿名化，而非样本级匿名化**

从结构视角（graph/process/topological evolution）构建宏观历史构象，而非传统的点对点脱敏。

**5 你个人已经做了哪些工作**

- 初步调研了隐私保护、时间序列隐私泄露、长期行为数据研究相关文献。
- 对现有的差分隐私与模型遗忘技术做了初步总结。
- 提出了三个潜在科研问题和一个核心理论贡献方向。




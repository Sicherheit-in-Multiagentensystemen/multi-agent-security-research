# 四阶段阅读路线

建议按理解深度推进，不要求固定每周完成篇数。括号内 ID 对应[文献库](../papers/README.md)。

| 阶段 | 建议阅读 | 应产出的文本 |
| --- | --- | --- |
| 1. 建立问题地图 | Open Challenges（P01）、Indirect Prompt Injection（P17）、Byzantine Generals（P21） | 一页研究边界、一个系统图、术语表 |
| 2. 理解传播与失效 | Prompt Infection（P02）、Agent Smith（P03）、CORBA（P04）、AgentPoison（P15）、Agents Under Siege（P06） | 对比攻击入口、传播机制与可观察后果的矩阵 |
| 3. 分析防御及其代价 | Security Tax（P05）、CaMeL（P16）、Can CaMeLs Talk?（P07）、G-Designer（P11） | 防御保证/假设表、正常效用损失清单 |
| 4. 形成最小实验 | InjecAgent（P12）、AgentDojo（P13）、ASB（P14）、Quantitative Benchmarking（P09）、Representation Sensitivity（P18） | 一份带对照和成功判据的实验方案 |

每篇先完成摘要级阅读卡片，优先对与选题直接相关的文章全文精读。论文的年份和发表状态在目录中逐篇查看，尤其注意近期预印本。

**串谋审计专题**：在第 2–4 阶段加入 Colosseum（P25），先读[论文卡片](../papers/notes/P25-colosseum.md)，再使用[审计框架](../frameworks/COLOSSEUM_AUDIT.md)对齐对话判分、行动 regret、联盟优势与公共目标损失。建议产出一份区分纸面串谋和实际行动的实验方案。

如果选择 MARL 或机器人方向，可先读 Adversarial Policies（P19）、Stochastic Adversary MARL（P20）与 IBGP（P10），再决定哪些 LLM 代理问题具有可比的威胁模型。HPTSA（P24）可作为多智能体安全任务能力的旁支阅读。

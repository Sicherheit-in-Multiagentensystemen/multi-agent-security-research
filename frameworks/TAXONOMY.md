# 文献分类框架

这是一套用于组织本仓库的工作分类，不是外部标准。分类采用多个轴；一篇论文可以拥有多个标签，不强行放入单一攻击类别。

## 六个记录轴

| 轴 | 需要记录的内容 | 示例 |
| --- | --- | --- |
| 系统结构 | 中心化、层级、点对点、市场式；静态/动态拓扑 | planner → workers |
| 攻击入口 | 用户输入、检索、工具、代理消息、共享记忆、注册与发现 | 被污染的工具结果 |
| 攻击者能力 | 控制对象、身份数、写入范围、轮次、预算、白盒/黑盒 | 可改一名 worker 的一条消息 |
| 失效机制 | 指令升级、身份冒充、委派越权、投毒、资源耗尽、串谋 | 下游把引用内容当成新指令 |
| 安全后果 | 外传、越权写入、目标劫持、错误共识、阻塞 | 未授权的外部工具调用 |
| 防御与证据 | 控制层、保证边界、评测条件、效用代价、复现状态 | 运行时权限策略与来源追踪 |

## 主题标签

| 标签 | 核心问题 | 起步文献 |
| --- | --- | --- |
| `injection-propagation` | 指令如何跨消息和代理传播？ | P02、P03、P06 |
| `availability` | 循环、递归和通信阻塞如何消耗资源？ | P04 |
| `memory-poisoning` | 记忆写入和后续检索如何改变行为？ | P15 |
| `identity-delegation` | 权限和来源能否跨代理边界保留？ | P07、P16；A2A、MCP 指南 |
| `collusion-coordination` | 联盟的通信与行动如何偏离公共目标？ | P01、P25；[Colosseum 审计框架](COLOSSEUM_AUDIT.md) |
| `robust-topology` | 通信结构如何影响攻击与防御？ | P06、P10、P11 |
| `security-utility` | 防御对正常协作造成什么损失？ | P05、P07 |
| `evaluation-validity` | 成功判据、环境和表示方式是否扭曲结论？ | P09、P12–P14、P18 |
| `marl-robustness` | 对手策略与观测扰动如何影响策略？ | P19、P20 |
| `byzantine-foundations` | 故障数量、同步与认证假设决定哪些保证？ | P21、P22 |

## 如何使用

每个论文条目先确定范围标签，再填写六轴。`未报告`表示原文未提供；`未核查`表示整理者尚未检查；`不适用`表示该项与研究对象无关。这三种状态不能互换。

在[证据矩阵](../papers/EVIDENCE_MATRIX.md)中记录最小索引，在阅读卡片中记录页码、表号与版本。跨论文比较前先对齐攻击能力、任务分布和预算。

外部框架仅用于交叉映射：用 [OWASP Agentic Security](https://genai.owasp.org/initiative_name/agentic-security/)核查风险类别，用 [MAESTRO](https://cloudsecurityalliance.org/blog/2025/02/06/agentic-ai-threat-modeling-framework-maestro)检查架构层次，用 [MITRE ATLAS](https://atlas.mitre.org/)关联攻击技术；不把这些映射当成实验证据。

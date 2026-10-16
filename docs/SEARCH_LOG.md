# 首批文献检索记录

整理日期：2026-10-16（Asia/Shanghai）。范围：多智能体系统安全研究的起步资料库。方法：定向检索、原始来源核对与少量引文/项目追踪；未执行穷尽式数据库导出，不声称 PRISMA 系统综述。

## 使用的查询示例

| 方向 | 查询词 |
| --- | --- |
| 研究地图 | `multi agent systems security survey 2025 2026` |
| 传播攻击 | `multi agent systems security prompt infection AgentSmith Corba benchmark` |
| 安全与协作 | `Multi-Agent Security Tax` |
| 工具与记忆 | `InjecAgent`、`AgentDojo`、`Agent Security Bench`、`AgentPoison` |
| 结构化防御 | `Defeating Prompt Injections by Design`、`Can CaMeLs Talk` |
| 评测有效性 | `multi agent security benchmark`、`Threat-Preserving Representation Sensitivity` |
| 分布式与 MARL | `The Byzantine Generals Problem`、`Byzantine Tolerant Gradient Descent`、`Robust Multi-Agent Reinforcement Learning` |
| 指南与协议 | `MAESTRO`、`OWASP Agentic`、`MCP security best practices`、`A2A security authentication` |

## 来源与核验

- arXiv：核对标题、作者、年份、摘要与可识别版本；仅凭 arXiv 页面不推断同行评审状态。
- ACL Anthology、PMLR、NeurIPS：核对已采用正式出版版本的元数据。
- Microsoft Research：核对拜占庭将军问题经典论文的作者与出版信息。
- 项目官方组织与仓库：核对资源链接、项目描述和可访问性；未运行代码。
- OWASP、CSA、MCP、A2A、MITRE、NIST：只使用官方来源说明对应资料的用途。

本次初筛未逐篇精读全文，因此不提取未核实的表号、实验数值或证明细节。条目中的“阅读问题”“局限提示”和研究路线属于整理者的研究建议。

## 已处理的版本差异

- **Agent Smith（P03）**：采用 ICML 2024 / PMLR 正式页面；同时保留 arXiv ID 作为关联标识。
- **Agents Under Siege（P06）**：采用 ACL 2025 正式页面。
- **AgentDojo（P13）**：以 arXiv 记录为目录来源，正式发表信息通过 NeurIPS 2024 论文核验；BibTeX 明确引用 arXiv 版本。
- **HPTSA（P24）**：采用 EACL 2026 正式页面。早期 2024 预印本与正式版作者、实验数量和结果不同，不混用。
- **2026-10 新文献（P07、P18）**：标注预印本，不把尚未复现的结果表述为本组织结论。

## 筛选边界

优先纳入直接 MAS 威胁、防御、评测与理论衔接。保留少量单 agent 安全基准和分布式基础，用范围标签说明迁移距离。没有把一般聊天越狱文章批量加入核心列表。

检索中出现的部分二手聚合页只用于发现，未作为最终论据。`Attention-based Fault-tolerant Approach for Multi-agent Reinforcement Learning Systems` 的 arXiv 页面包含管理员文本重叠提示，本次未纳入主清单；MARL 入口改选已核验的 ICML 2025 论文。该处理是本次资料筛选决定，不构成对论文研究有效性的独立裁定。

## 下轮更新需要补充

串谋与隐蔽通信、Sybil 与声誉攻击、隐私泄漏与推断、具身 MAS 的物理安全、A2A/MCP 的实证攻击防御、负结果与独立复现。下一轮须保存更完整的候选条目和排除原因，才能支持系统综述级别的覆盖声明。

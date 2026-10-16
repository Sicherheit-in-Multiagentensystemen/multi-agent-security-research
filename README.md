# 多智能体系统安全研究

**Sicherheit in Multiagentensystemen · Security in Multi-Agent Systems**

本仓库是多智能体系统安全课题的研究资料入口：收集原始文献、梳理威胁与防御、记录阅读证据，并为后续选题和复现实验提供可复用文本框架。正文以中文为主，保留英文标题和原始来源。

**首批整理日期：2026-10-16。** 当前收录 24 篇文献。条目已核对原始来源的元数据与摘要；均未在本组织完成复现实验。此清单是研究起点，不是系统性综述或完整文献全集。明确核验的会议/期刊版本会标注，其余 arXiv 条目标记为“正式发表状态未核验”。

## 从这里开始

| 你要做什么 | 入口 |
| --- | --- |
| 浏览分类文献与阅读问题 | [文献库](papers/README.md) |
| 找到原始引用与结构化数据 | [BibTeX](papers/references.bib) · [JSON 目录](papers/catalog.json) |
| 对比不同论文的假设与证据 | [文献证据矩阵](papers/EVIDENCE_MATRIX.md) |
| 看几篇关键论文的初步阅读卡片 | [起步笔记](papers/notes/README.md) |
| 统一课题范围和分类方式 | [研究范围](frameworks/RESEARCH_SCOPE.md) · [分类框架](frameworks/TAXONOMY.md) |
| 为具体系统建模 | [威胁建模框架](frameworks/THREAT_MODEL.md) |
| 开展规范的文献整理 | [文献综述流程](frameworks/LITERATURE_REVIEW.md) · [本次检索记录](docs/SEARCH_LOG.md) |
| 设计可比较的安全实验 | [评测框架](frameworks/EVALUATION.md) |
| 形成研究问题与近期计划 | [研究路线图](docs/ROADMAP.md) · [阅读路线](docs/READING_PATH.md) |
| 找安全指南、协议与开源基准 | [资料与工具](resources/README.md) |
| 新增论文或实验记录 | [贡献说明](CONTRIBUTING.md) · [模板目录](templates/README.md) |

## 研究主线

1. **传播与级联风险**：提示注入、记忆污染和可用性攻击如何从单个代理扩散到团队。
2. **身份、授权与委派**：代理之间如何表达权限、保留数据来源、限制工具能力。
3. **鲁棒协作与防御组合**：局部防御是否能组合为系统保证，防御如何影响正常协作。
4. **评测与可复现性**：同时测量攻击结果、传播范围、任务效用、预算与恢复能力。
5. **理论与传统 MAS 基础**：从拜占庭容错、鲁棒 MARL 和分布式学习中借鉴明确假设与证明方法。

文献中的作者结论、仓库整理者提出的延伸问题、以及本组织未来的复现结果必须分别记录。具体操作见[贡献说明](CONTRIBUTING.md)。

## 推荐起读

- [Open Challenges in Multi-Agent Security](https://arxiv.org/abs/2505.02077)：建立研究问题地图。
- [Prompt Infection](https://arxiv.org/abs/2410.07283)：理解智能体间的恶意指令传播。
- [Multi-Agent Security Tax](https://arxiv.org/abs/2502.19145)：同时考察安全收益与协作损失。
- [AgentDojo](https://arxiv.org/abs/2406.13352)：学习把工具执行、攻击结果与正常效用放在同一评测环境。
- [Can CaMeLs Talk?](https://arxiv.org/abs/2610.05640)：关注跨代理组合安全；2026-10 预印本，结论仍需独立验证。

## 仓库组织

```text
papers/        分类文献、引用、证据矩阵与起步笔记
resources/     指南、协议和开源基准
frameworks/    研究范围、分类、文献整理、威胁建模与评测文本
templates/     阅读卡片、威胁模型、实验记录、周报与综述提纲
docs/          阅读路线、研究计划与检索记录
```

论文与外部代码遵循各自版权和许可证。本仓库保存链接、引用及原创整理文本，不镜像第三方论文全文。后续更新通过提交记录追踪；目前未设置自动收集任务。

# P25 · Colosseum: Auditing Collusion in Cooperative Multi-Agent Systems

- 作者：Mason Nakamura、Abhinav Kumar、Saswat Das、Sahar Abdelnabi、Saaduddin Mahmud、Ferdinando Fioretto、Shlomo Zilberstein、Eugene Bagdasarian。
- 引用版本：[arXiv:2602.15198v2](https://arxiv.org/abs/2602.15198v2)，2026-05-27；首版发布于 2026-02-16。
- 官方代码：[umass-ai-safety/colosseum](https://github.com/umass-ai-safety/colosseum)，本次核查提交 `b077fe7e2f10566e92156cc12e06ffb2aac54790`。
- 发表信息：官方项目与[作者页面](https://saswatdas.com/publication/colosseum/)注明 NeurIPS 2026 Evaluations and Datasets Track 录用；本次引用 arXiv v2，未独立核验正式出版页。
- 范围：`direct-mas`；主题：`collusion-coordination`、`evaluation-validity`。
- 核验日期：2026-10-16。已核对元数据、摘要、方法/指标/局限章节及官方 README；尚未完成逐页全文精读、实现审查或实验复现。

## 研究问题

论文讨论合作任务中的联盟如何偏离共同目标。它把通信日志与实际行动分开审计：对话出现串谋迹象，并不意味着行动中实现了联盟优势；仅看对话也可能遗漏行动层面的异常。[原文 §3–5](https://arxiv.org/html/2602.15198v2)

## 方法索引

| 核对对象 | 原文位置 | 本组织记录 |
| --- | --- | --- |
| DCOP 任务与共同目标 | §3.1 | 为最终联合行动提供可计算的评价基础 |
| 联盟目标与混合目标 | §4.1–4.2 | 指定目标权重与实际行为需要区分 |
| 行动和通信指标 | §5.3 | 分别保留 regret、联盟优势、judge 评分 |
| 私有通道干预与对照 | §5.4、图 4 | “提供通道”是实验条件，不能写成无条件自发串谋 |
| 适用范围 | §6 Limitations and Future Work | 明确目标、可分解收益及短时任务；长程和异构团队需另行验证 |

这里提供证据定位，不转录论文的结果表。指标与复现实验的组织方式见[Colosseum 串谋审计框架](../../frameworks/COLOSSEUM_AUDIT.md)。

## 整理者的阅读与研究问题

1. 联盟优势变化能否排除初始能力、角色权限和额外通信预算的影响？
2. 对话 judge 与行动指标分歧时，是评判失误、协作失败，还是目标不可达？
3. 若公共目标本身不合理，如何区分有害串谋与合理的协同行为偏离？
4. 混合模型、跨任务记忆和长期委派会如何改变这一审计方法的适用条件？

这些是本组织提出的待验证问题，不是本文已经回答的普遍结论。

## 关联文献

- P01：系统层风险与串谋研究议程。
- P05：限制私有通信等措施可能影响正常协作，须同时衡量安全税。
- P09、P13：评测应追踪实际行动与最终任务状态。
- P10、P21：一致协调与目标符合性需要分别分析。

## 独立验证状态

未安装、运行或复现 Colosseum。后续使用[串谋审计实验模板](../../templates/COLLUSION_AUDIT.md)登记任务、对照、原始指标、归一化方式和日志。

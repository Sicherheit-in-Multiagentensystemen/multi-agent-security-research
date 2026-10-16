# P07 · Can CaMeLs Talk? Securing Multi-Agent Systems Against Indirect Prompt Injection Attacks

- 原始来源：[Can CaMeLs Talk?](https://arxiv.org/abs/2610.05640)
- 作者：Peters-Gill, James; Semler, Avi; Bartsch, Henning; Shumailov, Ilia; de Witt, Christian Schroeder
- 年份/发表状态：2026；预印本
- 所用记录：v1；核验日期 2026-10-16
- 范围：`direct-mas`
- 阅读状态：`metadata-and-abstract-checked`
- 代码检查：尚未进行；复现：`not-reproduced`

## 原文摘要层面的内容

讨论单智能体 CaMeL 保证在层级多智能体组合时的失效，并提出跨代理保留来源信息的 multi-CaMeL。

## 整理者解读

重点检查跨代理调用时，原本带有不可信来源的数据是否被下游重新解释成可信任务；单组件保证不自动组合。

## 适用边界

2026-10 新预印本；实验中的零成功攻击不代表对任意攻击的无条件保证。

## 全文精读时要回答

1. 下游代理是否会把上游不可信数据重新当成可信指令？
2. 系统和攻击者的精确假设是什么？请记录页码、节号或表号。
3. 什么反例或配置变化可能使结论失效？是否报告正常任务表现与资源成本？

## 下一步文本产出

精读后提取协议中指令和数据通道的定义、来源传播规则及信任假设；当前尚未检查实现。

## 证据与独立验证

具体页码、表格和数值：未核查。代码提交和实验日志：尚无。本卡片不提供独立复现结论。

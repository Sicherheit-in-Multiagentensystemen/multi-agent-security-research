# P13 · AgentDojo: A Dynamic Environment to Evaluate Prompt Injection Attacks and Defenses for LLM Agents

- 原始来源：[AgentDojo](https://arxiv.org/abs/2406.13352)
- 作者：Debenedetti, Edoardo; Zhang, Jie; Balunović, Mislav; Beurer-Kellner, Luca; Fischer, Marc; Tramèr, Florian
- 年份/发表状态：2024；已核验发表
- 所用记录：v3；核验日期 2026-10-16
- 范围：`transferable-agent`
- 阅读状态：`metadata-and-abstract-checked`
- 代码检查：尚未进行；复现：`not-reproduced`

## 原文摘要层面的内容

提供工具、任务、攻击与防御共同运行的可扩展环境，支持同时测量安全与正常任务表现。

## 整理者解读

以工具与环境的实际状态核验任务和攻击结果，防止把模型声称完成与真实副作用混为一谈。

## 适用边界

原始环境不是多智能体传播评测；扩展时需记录代理边界与消息路径。

## 全文精读时要回答

1. 攻击是否真正改变环境状态，还是只诱导模型输出文本？
2. 系统和攻击者的精确假设是什么？请记录页码、节号或表号。
3. 什么反例或配置变化可能使结论失效？是否报告正常任务表现与资源成本？

## 下一步文本产出

选一个基准任务，先记录其无攻击可完成性，再设计增加代理边界后的同任务比较；本仓库尚未运行。

## 证据与独立验证

具体页码、表格和数值：未核查。代码提交和实验日志：尚无。本卡片不提供独立复现结论。

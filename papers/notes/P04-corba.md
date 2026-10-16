# P04 · CORBA: Contagious Recursive Blocking Attacks on Multi-Agent Systems Based on Large Language Models

- 原始来源：[CORBA](https://arxiv.org/abs/2502.14529)
- 作者：Zhou, Zhenhong; Li, Zherui; Zhang, Jie; Zhang, Yuanhe; Wang, Kun; Liu, Yang; Guo, Qing
- 年份/发表状态：2025；arXiv；正式发表状态未核验
- 所用记录：v1；核验日期 2026-10-16
- 范围：`direct-mas`
- 阅读状态：`metadata-and-abstract-checked`
- 代码检查：尚未进行；复现：`not-reproduced`

## 原文摘要层面的内容

研究递归阻塞指令在多智能体系统中的传播及资源消耗。

## 整理者解读

把内容危害与系统可用性分开：一条指令即使不要求有害输出，也可能诱导无界循环或递归等待。

## 适用边界

阻塞、超时与任务失败应分别记录，不能统一算作越狱。

## 全文精读时要回答

1. 当内容看似无害但使系统持续等待或循环时，应如何判定可用性损失？
2. 系统和攻击者的精确假设是什么？请记录页码、节号或表号。
3. 什么反例或配置变化可能使结论失效？是否报告正常任务表现与资源成本？

## 下一步文本产出

定义一个有界任务的时间、调用次数和预算阈值，列出超时、正常终止与工具错误的不同判据。

## 证据与独立验证

具体页码、表格和数值：未核查。代码提交和实验日志：尚无。本卡片不提供独立复现结论。

# 研究范围与术语

## 工作定义

本组织研究多个自主或半自主智能体在通信、共享环境、共享记忆或委派工具权限时产生或放大的安全风险。核心问题是：一个局部可控的输入、消息或节点，如何改变整个系统的安全属性？

以 LLM 多智能体系统为当前重点，同时保留传统 MAS、MARL 和分布式系统基础。网络安全任务中的多智能体工具另设“安全应用”标签，避免将应用能力误当成系统防御证据。

## 五类文献范围

| 标签 | 定义 | 例子 |
| --- | --- | --- |
| `direct-mas` | 直接研究多智能体交互或系统层安全/鲁棒性 | Prompt Infection、CORBA、IBGP |
| `transferable-agent` | 单智能体或通用 agentic 安全，可迁移到 MAS 但需验证 | AgentDojo、CaMeL、AgentPoison |
| `marl` | 多智能体强化学习的对抗策略或鲁棒性 | Adversarial Policies、Stochastic Adversary MARL |
| `distributed-foundation` | 容错、共识、分布式聚合等理论基础 | Byzantine Generals、Krum |
| `security-application` | 利用多智能体完成网络安全等任务 | HPTSA |

## 安全属性

- **机密性**：未经授权的主体不能获得私密信息。
- **完整性**：系统目标、消息、记忆和输出不被未授权地改变。
- **可用性**：系统能在限定资源和时间内继续完成任务或有界终止。
- **身份与授权**：知道消息的来源，并检查该主体是否有权触发具体操作。
- **可追溯性**：能重建消息、委派、工具调用与最终副作用之间的链路。
- **安全性与可靠性**：有害行为、非恶意错误和任务失败分别记录；不能默认失败由攻击引起。

## 需要区分的概念

1. 多代理投票形成一致意见，不自动保证事实正确或操作已授权。
2. TLS、签名和认证能保护通道或身份；已认证代理仍可能发送被污染的内容。
3. 内容审查模型的拒绝率不等于系统没有执行越权工具调用。
4. 单代理防御的实验成功不自动意味着在委派链中具有组合安全。
5. 鲁棒 MARL 中的观测扰动集合与 LLM 消息注入的攻击空间需要分别定义。

以上范围是本仓库的组织约定。研究议程参考 [Open Challenges](https://arxiv.org/abs/2505.02077)；组合安全问题参考 [Can CaMeLs Talk?](https://arxiv.org/abs/2610.05640)；协议假设分析参考 [The Byzantine Generals Problem](https://www.microsoft.com/en-us/research/publication/byzantine-generals-problem/)。

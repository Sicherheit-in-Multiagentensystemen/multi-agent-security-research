# 资料、协议与开源基准

核验日期：2026-10-16。以下 13 项来自官方来源。链接可用不等于代码已运行、许可证已审计或系统具备完整防御；开始实验前应固定提交、版本和依赖。

## 官方指南与协议

| 资料 | 用途 | 使用边界 |
| --- | --- | --- |
| [OWASP Agentic Security Initiative](https://genai.owasp.org/initiative_name/agentic-security/) | 检查目标劫持、权限、记忆、代理通信和级联风险等类别 | 风险清单和指导文档，不是本组织的实测得分 |
| [CSA MAESTRO](https://cloudsecurityalliance.org/blog/2025/02/06/agentic-ai-threat-modeling-framework-maestro) | 按架构层次开展威胁建模，识别跨层攻击链 | 具体覆盖需结合实际系统，不能直接产生安全保证 |
| [MCP Security Best Practices（2025-11-25 文档路径）](https://modelcontextprotocol.io/docs/2025-11-25/tutorials/security/security_best_practices) | 研究代理访问工具与服务时的授权和信任问题 | MCP 工具连接与 agent-to-agent 委派需分别分析；文档会更新 |
| [A2A Enterprise Features](https://a2a-protocol.org/latest/topics/enterprise-ready/) | 理解代理协作中的认证、授权与企业部署关注点 | `latest` 是动态页面，实施时固定协议版本；认证不保证内容可信 |
| [MITRE ATLAS](https://atlas.mitre.org/) | 给 AI 系统攻击技术建立可追踪的映射 | 映射到攻击技术不等于已经实证覆盖该技术 |
| [NIST AI Risk Management Framework](https://www.nist.gov/itl/ai-risk-management-framework) | 连接系统风险、测量、管理与治理活动 | 通用风险管理框架，需补充 MAS 技术威胁模型 |

## 官方开源研究资源

| 项目 | 对应文献 | 适合做什么 | 边界 |
| --- | --- | --- | --- |
| [CORBA](https://github.com/zhrli324/Corba) | P04 | 研究多代理递归阻塞与可用性 | 阅读实验设置后再复现，不把阻塞计为所有类型攻击成功 |
| [InjecAgent](https://github.com/uiuc-kang-lab/InjecAgent) | P12 | 工具返回内容中的间接提示注入 | 原始基准不衡量完整的 MAS 传播 |
| [AgentDojo](https://github.com/ethz-spylab/agentdojo) | P13 | 任务、工具、攻击与防御联合评测 | 原始环境需扩展才能测试代理间传播 |
| [Agent Security Bench](https://github.com/agiresearch/ASB) | P14 | 比较多个攻击面和防御类型 | 场景、指标和代码版本需要同时锁定 |
| [CaMeL](https://github.com/google-research/camel-prompt-injection) | P16 | 理解控制/数据流分离与权限策略 | 不同于 CAMEL 多代理协作框架；组合安全需独立分析 |
| [HPTSA](https://github.com/uiuc-kang-lab/HPTSA) | P24 | 分析团队规划与安全任务能力 | 安全应用资料，与保护 MAS 的防御证据分开存放 |
| [Colosseum](https://github.com/umass-ai-safety/colosseum) | P25 | 联合审计串谋对话与实际联盟行动 | 记录论文 v2 与代码提交，区分原始/归一化指标；配套[审计框架](../frameworks/COLOSSEUM_AUDIT.md) |

本组织当前没有运行上述项目，也没有已完成的安全实验。实验状态以[文献目录](../papers/catalog.json)和后续实验记录为准。

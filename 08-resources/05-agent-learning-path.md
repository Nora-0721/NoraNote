# Agent 资源学习路径

## 面试前最小顺序

1. [OpenAI 实用 Agent 指南](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/)：先看 Agent 定义、何时该用 Agent、模型/工具/指令和单 Agent 循环。
2. [MCP 架构](https://modelcontextprotocol.io/docs/learn/architecture)：只看 host/client/server 与 tools/resources/prompts。
3. [OpenAI 开发者资源中的 Building agents 学习路径](https://developers.openai.com/resources/)：需要动手时再进入 Responses 与工具示例。
4. 回到 [Agent 后端服务架构](../06-agent-engineering/05-agent-backend-service-architecture.md)，把 HTTP、数据库、任务队列、超时和 tracing 串起来。

## 面试边界

- Agent 不是普通聊天机器人，也不是所有工作流都需要 Agent。
- Tool Use 是模型选择并调用外部能力；MCP 是暴露上下文和工具的协议边界。
- RAG、Context、Memory 不互相等价。
- 先讲自己真实使用 Codex/Agent 完成仓库分析和文档整理的经历，不把没做过的多 Agent 系统说成项目经验。

完整任务入口：[7 月 22 日](./02-july-18-to-24-must-use.md#2026-07-22) · [Agent 专栏](../06-agent-engineering/README.md)

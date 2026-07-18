# 项目、后端与支付资源路径

## 项目先于教程

- SLAM：先画本人三端链路，再用 [7 月 18 日](./02-july-18-to-24-must-use.md#2026-07-18) 的 OpenGL 官方页校准线程与 Renderer 术语；7 月 21 日回到 Profiler 和项目代码补证据。
- AI 命理平台：先沿真实业务链路画上传、生成、持久化和支付解锁；后端资料只用于解释本人确实做过的部分。
- 两个项目都必须准备 [真实性边界与指标证据](../03-resume-projects/06-truth-boundaries-and-metrics.md)。

## 后端最小链路

1. [7 月 22 日](./02-july-18-to-24-must-use.md#2026-07-22)：HTTP、鉴权、事务、索引。
2. [7 月 23 日](./02-july-18-to-24-must-use.md#2026-07-23)：Django、Redis、异步任务与重试。
3. 只回答这些能力怎样支撑 Agent、AI 报告任务和支付通知，不扩展成完整后端八股。

## 支付最小链路

1. 本地订单与 Stripe Checkout/PaymentIntent。
2. Webhook 原始请求体验签、快速返回 2xx。
3. 事件去重、数据库事务和状态机。
4. 7 月 24 日后再看退款、争议和对账。

文章入口：[简历项目](../03-resume-projects/README.md) · [后端底座](../04-backend-for-agent-and-payment/README.md) · [支付工程](../05-payment-engineering/README.md)

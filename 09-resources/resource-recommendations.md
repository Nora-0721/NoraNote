# 安卓应面 + Agent/支付 速通推荐资源清单

> 更新日期：2026-07-18  
> 说明：优先选择讲解清晰、适合面试速通的文章与官方文档。国内以掘金、CSDN、知乎为主，国外以官方文档 + 经典图解为主。每个知识点尽量提供 2–4 个优质链接。

---

## 使用建议（匹配速通节奏）

1. **7/18–7/20**：优先刷 Activity + Handler + 四大组件 + 网络基础（推荐掘金鹏程十八少系列）。
2. **7/21–7/22**：Compose + MVVM + Retrofit 标准链路。
3. **7/23**：支付状态机 + Webhook 幂等 + Agent 一句话解释 + 项目追问话术。
4. 每个知识点准备 **30 秒版 + 2 分钟版**，面试先短答再展开。

---

## Android 基础八股（P0）

### 1.1 Activity 生命周期与启动模式

- [深度解析 Android Activity 启动模式：从生命周期到任务栈](https://juejin.cn/post/7470849622689497126)（掘金，图解清晰）
- [【Android】活动的正/异常生命周期和启动模式详解](https://juejin.cn/post/7568873939033833522)
- [Activity 生命周期和启动模式 —— 重读《Android 开发艺术探索》](https://juejin.cn/post/7077503479240982535)
- 官方文档：[Activity lifecycle](https://developer.android.com/guide/components/activities/activity-lifecycle)

### 1.2 Handler 机制、内存泄漏与 ANR

- [Android Handler 完全指南：28 道高频面试题 + 源码解析 + 图解](https://juejin.cn/user/184373685534077)（鹏程十八少系列，强烈推荐）
- [Handler 消息机制-简要版](https://juejin.cn/post/7340926094613135370)
- [手把手带你看源码：一文说透 Handler 原理](https://juejin.cn/post/6844904164296753166)
- [Handler 面试必问八大题](https://blog.nowcoder.net/n/5296fffbf37148c786b416f6f6abc0a8)

### 1.3 四大组件、权限、存储、网络基础

- [安卓面试八股文整理（基础组件篇）](https://blog.csdn.net/ass133755/article/details/155752650)
- 官方权限与分区存储：Android Developers 搜索 “Permissions” / “Scoped Storage”
- HTTPS / TCP 基础：[小林coding - TCP 三次握手与四次挥手](https://www.xiaolincoding.com/network/3_tcp/tcp_interview.html)

### 1.4 RecyclerView、自定义 View、事件分发

- 掘金搜索「鹏程十八少 RecyclerView」「鹏程十八少 自定义 View」（高频面试题系列）
- 经典参考：《Android 开发艺术探索》相关章节总结（掘金大量优质转载）

---

## MVVM / Jetpack / 现代架构（P0–P1）

- 官方：[Android App Architecture](https://developer.android.com/topic/architecture)
- 官方：[UI layer](https://developer.android.com/topic/architecture/ui-layer)
- 官方：[Data layer](https://developer.android.com/topic/architecture/data-layer)
- [Android Jetpack Compose + MVVM 开发流程深度分析](https://juejin.cn/post/7529753631354109992)
- 官方：[ViewModel overview](https://developer.android.com/topic/libraries/architecture/viewmodel)

---

## Jetpack Compose 速通（P0）

### 官方核心文档（必看）

- [Compose State](https://developer.android.com/develop/ui/compose/state)
- [State Hoisting](https://developer.android.com/develop/ui/compose/state-hoisting)
- [Compose Architecture](https://developer.android.com/develop/ui/compose/architecture)
- [Thinking in Compose](https://developer.android.com/develop/ui/compose/mental-model)

### 视频补充

- YouTube 搜索 “Compose + MVVM + Hilt + Room 2025/2026”（推荐 UiLover 等频道最新教程）

---

## Retrofit / OkHttp 网络层（P0）

- [Retrofit + OkHttp 网络请求](https://juejin.cn/post/7652270980880547840)（基础清晰）
- [2026 金三银四 Android OkHttp 面试核心 45 问](https://juejin.cn/post/7631311804195094564)（鹏程十八少）
- [OkHttp 架构剖析：从拦截器链到连接池](https://juejin.cn/post/7634002571019288595)
- 官方：[Retrofit](https://square.github.io/retrofit/)
- 官方：OkHttp 文档

---

## 支付工程（Stripe）速通（P0–P1）

### 官方必看

- [Stripe Webhooks](https://docs.stripe.com/webhooks)
- [Idempotent Requests](https://docs.stripe.com/api/idempotent_requests)
- [Checkout Sessions](https://docs.stripe.com/api/checkout/sessions/create)
- [Payment Intents](https://docs.stripe.com/payments/payment-intents)
- [Key best practices](https://docs.stripe.com/keys-best-practices)

### 生产级实践文章（强烈推荐）

- [Stripe Webhooks in Production: The Idempotency Guide](https://dev.to/whoffagents/stripe-webhooks-in-production-the-idempotency-guide-nobody-writes-513k)
- [Webhook Idempotency Is Not Optional](https://fourteensystems.com/blog/webhook-idempotency-is-not-optional)
- [Stripe Webhook Best Practices 2026](https://hookray.com/blog/stripe-webhook-best-practices-2026)

---

## Agent 开发速通（P1–P2）

### 核心概念（ReAct / Tool Use / Harness）

- [从零玩转 Agent 开发：原理、架构与框架实战完全指南](https://juejin.cn/post/7659251251616202779)（六层架构图清晰）
- [保姆级复盘：手写 LangChain 工具调用 Agent，吃透 ReAct](https://juejin.cn/post/7659671273129443378)
- [ReAct Agent 深度解析 2026](https://juejin.cn/post/7634469727899205667)
- [从 CoT 到 ReAct：AI Agent 是怎么“长出来”的](https://juejin.cn/post/7660513725812785202)

### Transformer 基础

- **最推荐**：[The Illustrated Transformer](https://jalammar.github.io/illustrated-transformer/)（经典图解，中文翻译版很多）
- B站搜索「李宏毅 Transformer」

### MCP / Skills / Tool Use

- OpenAI 官方：

  - [Function Calling](https://developers.openai.com/api/docs/guides/function-calling)
  - [MCP Guide](https://developers.openai.com/api/docs/mcp)
  - [Tools / Skills](https://developers.openai.com/api/docs/guides/tools-skills)
- 掘金搜索「MCP Agent」或「Skills Agent」最新文章

### Agent Harness 相关

- [What is an AI Agent Harness?（Databricks）](https://www.databricks.com/blog/ai-harness)
- [从零设计生产级 Multi-Agent Harness](https://cloud.tencent.com/developer/article/2668186)（腾讯云）

---

## Java 基础八股（P0）

- 掘金搜索「2026版 Java 八股面试文」
- [JavaGuide](https://javaguide.cn/)（经典全面）
- HashMap / 并发 / JVM 推荐「小林coding」或美团技术团队相关文章

---

## 后端基础（Django + 支付相关）

- Django 官方文档：[docs.djangoproject.com](https://docs.djangoproject.com/)
- 掘金搜索「Django 请求生命周期」
- CSDN / 掘金「Django ORM 全面解析」
- 支付状态机 + 幂等：参考上方 Stripe 生产级文章
- 订单超时自动取消方案对比：掘金搜索「订单超时自动取消」

---

## 综合面试题与知识体系

- 掘金搜索「鹏程十八少」（Android 高频面试题系列持续更新）
- [GitHub - CommonDevKnowledge（BAT 面试题汇集）](https://github.com/AweiLoveAndroid/CommonDevKnowledge)
- Android 官方架构与 Compose 文档合集（优先看官方）

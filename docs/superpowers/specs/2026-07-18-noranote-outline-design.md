# NoraNote 面试速通目录设计

## 1. 目标

NoraNote 是一套以个人求职冲刺为第一目标、后续可供同学复用的面试笔记目录。

- 2026-07-24 前完成 Android 首轮面试的 P0 防线。
- 2026-08-05 前以获得第一个 Offer 为目标，边面试边补 P1/P2。
- 主投 Android 客户端，辅投 Agent 开发。
- 后端不是独立求职主线，而是 Agent 岗位、AI 命理平台和 Stripe 支付项目的共同工程底座。
- 当前阶段只建立目录、导航、优先级和文章产物，不写正文。

## 2. 设计原则

采用“冲刺入口 + 知识专栏”的双层导航：

1. README 首屏回答今天学什么、7 月 24 日前必须会什么。
2. 专栏地图保留 X-Plore 的“专栏 → 文章”浏览体验。
3. 日期视图和知识视图链接到同一篇文章，不重复维护正文。
4. P0/P1/P2 写在导航表中，不写进文件名，保证链接稳定。
5. 文章粒度以能独立复习、口述或分享为准。
6. 资源必须服务于具体任务，不能把搜索词、作者主页或泛泛首页当作推荐条目。

## 3. 信息架构

```text
NoraNote/
├─ README.md
├─ daily-plan.md
├─ article-template.md
│
├─ 00-start-here/
│  ├─ README.md
│  ├─ 01-target-roles-and-boundaries.md
│  ├─ 02-p0-p1-p2-priority-map.md
│  ├─ 03-july-18-to-24-sprint.md
│  └─ 04-thirty-second-two-minute-answer.md
│
├─ 01-android-foundation/
│  ├─ README.md
│  ├─ 01-java-kotlin-minimum-pack.md
│  ├─ 02-collections-jvm-concurrency.md
│  ├─ 03-activity-lifecycle-task-stack.md
│  ├─ 04-fragment-and-four-components.md
│  ├─ 05-handler-looper-messagequeue.md
│  ├─ 06-threading-anr-and-memory-leaks.md
│  ├─ 07-recyclerview-custom-view-touch.md
│  └─ 08-permissions-storage-and-process.md
│
├─ 02-android-modern-stack/
│  ├─ README.md
│  ├─ 01-coroutines-and-structured-concurrency.md
│  ├─ 02-flow-stateflow-and-ui-state.md
│  ├─ 03-mvvm-udf-and-repository.md
│  ├─ 04-compose-state-recomposition-effects.md
│  ├─ 05-retrofit-okhttp-request-chain.md
│  ├─ 06-room-navigation-hilt-workmanager.md
│  └─ 07-compose-mvvm-retrofit-demo-map.md
│
├─ 03-resume-projects/
│  ├─ README.md
│  ├─ 01-project-answer-framework.md
│  ├─ 02-slam-system-and-data-flow.md
│  ├─ 03-slam-thread-render-memory.md
│  ├─ 04-ai-platform-business-loop.md
│  ├─ 05-ai-output-persistence-and-cost.md
│  └─ 06-truth-boundaries-and-metrics.md
│
├─ 04-backend-for-agent-and-payment/
│  ├─ README.md
│  ├─ 01-http-rest-auth-and-security.md
│  ├─ 02-django-request-and-service-layers.md
│  ├─ 03-data-model-transactions-and-indexes.md
│  ├─ 04-redis-cache-and-consistency.md
│  ├─ 05-async-jobs-retry-and-idempotency.md
│  └─ 06-logging-tracing-deployment.md
│
├─ 05-payment-engineering/
│  ├─ README.md
│  ├─ 01-order-payment-and-ledger-models.md
│  ├─ 02-stripe-checkout-paymentintent-flow.md
│  ├─ 03-webhook-signature-and-idempotency.md
│  ├─ 04-payment-state-machine-and-transactions.md
│  ├─ 05-refund-reconciliation-and-recovery.md
│  └─ 06-payment-interview-defense.md
│
├─ 06-agent-engineering/
│  ├─ README.md
│  ├─ 01-agent-workflow-and-agent-loop.md
│  ├─ 02-tool-use-and-function-calling.md
│  ├─ 03-mcp-resources-tools-and-prompts.md
│  ├─ 04-rag-context-and-memory.md
│  ├─ 05-agent-backend-service-architecture.md
│  ├─ 06-evals-tracing-and-guardrails.md
│  └─ 07-agent-interview-defense.md
│
├─ 07-interview-drills/
│  ├─ README.md
│  ├─ 01-android-p0-recite-list.md
│  ├─ 02-project-follow-up-list.md
│  ├─ 03-backend-payment-agent-list.md
│  ├─ 04-mock-interview-rounds.md
│  └─ 05-mistakes-and-post-interview-review.md
│
└─ 08-resources/
   ├─ README.md
   ├─ 01-resource-selection-rules.md
   ├─ 02-july-18-to-24-must-use.md
   ├─ 03-android-learning-path.md
   ├─ 04-project-backend-payment-path.md
   ├─ 05-agent-learning-path.md
   └─ 06-after-july-24-reference.md
```

## 4. 专栏边界

### 00 Start Here

只放目标、优先级、七日冲刺路线和统一答题方法。它负责把人送到正确文章，不承载技术正文。

### 01 Android Foundation

覆盖 Android 首面所需的语言与平台基础。Java 仅保留语言、集合、JVM 和并发的最小防线，不再作为平行主线。

### 02 Android Modern Stack

覆盖现代 Android 项目的状态、架构、网络与 Jetpack 组件，并用一篇 demo 地图串起 Compose、MVVM 和 Retrofit，但当前不实现 demo。

### 03 Resume Projects

围绕简历上的 SLAM Android 客户端和 AI 命理平台组织。回答必须区分真实职责、系统链路、技术取舍和指标证据。

### 04 Backend for Agent and Payment

覆盖 Agent 服务、AI 平台和支付共同需要的 Web/API、数据、异步、可靠性和可观测能力，不扩展成完整后端求职路线。

### 05 Payment Engineering

以本地订单为核心，串联 Stripe Checkout、PaymentIntent、Webhook、幂等、状态机、退款和对账。

### 06 Agent Engineering

从 Agent 与工作流的边界开始，覆盖工具调用、MCP、RAG、上下文、后端服务、评估和可观测性。避免把模型术语堆成无工程落点的词表。

### 07 Interview Drills

只放可直接练习和复盘的清单、模拟轮次及错题记录，不复制知识文章正文。

### 08 Resources

资源按冲刺任务和学习路径组织，而不是按网站或作者分类。

## 5. README 导航

README 按以下顺序呈现：

1. 一句话定位和两个硬截止日期。
2. “现在开始”快捷入口：今日任务、P0 背诵、项目追问、资源清单、面试复盘。
3. 7/18–7/24 七日冲刺表，只展示每日目标、预计时间、文章入口和完成产物。
4. 九个专栏的四列表格地图。
5. 7 月 24 日后的 P1/P2 补强路线。
6. GitHub 与飞书的分工、同步状态和使用说明。

完整的 7/18–8/05 日程保留在 `daily-plan.md`，不再复制到 README。

## 6. 专栏 README 与文章占位

每个专栏 README 使用同一导航表：

| 优先级 | 文章 | 预计用时 | 学完产物 | 状态 |
| --- | --- | ---: | --- | --- |
| P0 | Handler / Looper / MessageQueue | 45 分钟 | 30 秒口述 + 线程图 | 待写 |

当前阶段的文章文件只包含：

- 文章标题。
- P0/P1/P2 优先级。
- 预计学习或复习时间。
- 后续正文需要交付的产物，例如口述、流程图、代码链路或追问清单。
- “正文待写”状态。

不提前填写知识点正文。

## 7. 日程视图

`daily-plan.md` 每个任务使用以下字段：

- 日期和任务编号。
- 阶段与 P0/P1/P2。
- 预计用时。
- 对应的唯一文章链接。
- 精确资源链接。
- 当天完成产物。
- 完成状态。
- 面试后是否需要返工。

7/18–7/23 优先完成 Android P0 和项目防线；支付、Agent 及后端只保留简历和岗位要求所需的最小闭环。7/24 后再扩展 P1/P2。

## 8. 资源筛选与结构

每条推荐资源必须记录：

- 对应任务编号与文章。
- 资源类型：图解、视频、codelab、官方文档或项目示例。
- 建议阅读或观看范围。
- 预计耗时。
- 配图或演示程度。
- 看完能够回答的问题。
- 是否为一手资料。
- 链接核验日期。

筛选顺序：

1. 有明确时长、步骤和可见产出的官方课程或 codelab。
2. 有架构图、时序图、代码演示或项目成品的一手资料。
3. 能补充中文解释的高质量二手资料。
4. 长篇参考文档只放在 7 月 24 日后资源区。

删除或替换以下条目：

- 只有搜索关键词、没有精确链接的条目。
- 作者主页或站点首页冒充具体教程的条目。
- 重复资源。
- 未经核验的“2026 最新”“强烈推荐”等营销式描述。
- 与七日冲刺产物没有对应关系的泛泛收藏。

## 9. GitHub 与飞书同步

- GitHub 是文章目录、稳定链接和长期笔记的主版本。
- 飞书多维表格负责日程、完成状态和临时调整。
- 飞书资源推荐负责手机端快速打开资源，并链接到对应 GitHub 文章。
- 同一知识点只在 GitHub 保留一个正文来源。
- GitHub 文章路径确定后，更新飞书日程和资源表中的快捷链接。

当前环境能够读取三个公开飞书页面，但没有飞书编辑连接器或登录写入接口。因此实施阶段先完成 GitHub、资源候选表和可复制到飞书的更新内容；飞书实际写回需要可编辑连接方式。

## 10. 迁移策略

1. 建立新目录和占位文章。
2. 将现有文章按主题映射到新路径，避免知识主题重复。
3. 重写根 README 和各专栏 README。
4. 更新 `daily-plan.md` 的文章链接、资源链接和完成产物。
5. 重建资源索引，删除失效、泛泛或未经核验的推荐。
6. 删除被新结构替代的旧目录和同步占位文件。
7. 生成飞书更新清单。

迁移只处理框架和导航，不补知识正文。

## 11. 验收标准

- 每个 7/18–7/23 的 P0 任务都有唯一文章入口、精确资源入口和完成产物。
- 所有 Markdown 内链有效。
- 不存在孤立文章、重复主题或旧路径残留。
- README、专栏 README 和 `daily-plan.md` 的名称与链接一致。
- 外部推荐链接能够打开，并符合速通、图解或演示要求。
- 文章文件只有标题、优先级、预计时间、预期产物和待写状态，没有提前填正文。
- Android 是首屏主线；Agent 是辅投方向；后端明确作为 Agent、AI 平台和支付的工程底座。
- GitHub 与飞书的主数据边界写清楚，无法自动写回飞书时有可复制的更新清单。

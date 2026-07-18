# NoraNote

Android 面试速通与项目追问笔记仓库。

Core: Document everything - recording the learning process itself is a contribution.

- 按照“专栏 -> 文章”结构组织，点击可以直接跳转到对应文章。
- 当前阶段只定目录框架，不写正文内容。
- 主线：Android 客户端面试速通；辅线：Agent 开发、支付工程、Java/后端补位。

| 专栏 | 专栏 | 专栏 | 专栏 |
| --- | --- | --- | --- |
| [目标校正](00-goals-and-date/README.md) | [总体顺序](01-learning-order/README.md) | [Android 基础八股](02-android-basics/README.md) | [MVVM / Jetpack](03-mvvm-jetpack-architecture/README.md) |
| [Jetpack Compose](04-jetpack-compose/README.md) | [Retrofit / OkHttp](05-retrofit-okhttp-network/README.md) | [简历项目追问](06-resume-project-defense/README.md) | [支付工程](07-payment-engineering/README.md) |
| [Agent 开发](08-agent-development/README.md) | [推荐资料](09-resources/README.md) | [背诵清单](10-recite-checklist/README.md) | [面试策略](11-interview-strategy/README.md) |
| [Java 八股](12-java-basics/README.md) | [后端基础](13-backend-basics/README.md) | [多维表格](table-sync-placeholder.md) | [写作模板](article-template.md) |

### 日期 & 每日任务快捷导航

- 来源：[飞书多维表格：安卓应面 + Agent/支付速通计划表](https://gcnbv9droju6.feishu.cn/wiki/Vq2gwpGSaibpF3kfKy8chSiDnid)
- 完整任务表：[daily-plan.md](daily-plan.md)
- 完整资源清单：[09-resources/resource-recommendations.md](09-resources/resource-recommendations.md)

| 日期 | 阶段 | 当日主线 | 快捷 MD 笔记 | 推荐教程/资料 |
| --- | --- | --- | --- | --- |
| 2026-07-18 周六 | 投递前抢救 | 整理简历防线和提问清单；Java/Kotlin 面试最小包；Activity 生命周期 + 启动模式；等 6 项 | [项目回答](06-resume-project-defense/03-project-three-part-answer.md) / [算法/背诵](10-recite-checklist/01-android-high-frequency.md) / [Java/Kotlin](02-android-basics/01-java-kotlin-minimum-defense.md) / [集合](12-java-basics/02-java-collections.md) / [JVM/GC](12-java-basics/03-jvm-gc-minimum-defense.md) | 速通目录文档 / [教程](https://kotlinlang.org/docs/home.html) |
| 2026-07-19 周日 | 投递前抢救 | Java八股：集合框架和 HashMap；四大组件/权限/存储；UI/XML/RecyclerView/自定义 View；等 7 项 | [Java八股](12-java-basics/README.md) / [集合](12-java-basics/02-java-collections.md) / [四大组件](02-android-basics/02-android-components-lifecycle.md) / [权限/存储](02-android-basics/05-permission-storage-network.md) | JavaGuide + 美团技术团队 / [教程](https://developer.android.com/develop/background-work/background-tasks/broadcasts) |
| 2026-07-20 周一 | 面试前背诵 | Java八股：并发/JUC 最小防线；继续投递并记录岗位 JD；Compose 基础；等 6 项 | [Java八股](12-java-basics/README.md) / [JUC](12-java-basics/04-concurrency-juc-minimum-defense.md) / [协程/错误处理](05-retrofit-okhttp-network/03-interceptor-error-coroutine.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | Oracle concurrency tutorial / 招聘平台 |
| 2026-07-21 周二 | 面试前背诵 | Java八股：口述检测；协程/Flow/StateFlow；SLAM 项目深挖；等 5 项 | [Java八股](12-java-basics/README.md) / [集合](12-java-basics/02-java-collections.md) / [MVVM](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md) / [ViewModel/Flow](03-mvvm-jetpack-architecture/02-viewmodel-livedata-flow-stateflow.md) / [Compose](04-jetpack-compose/01-compose-core-concepts.md) | 错题本 / [教程](https://developer.android.com/kotlin/coroutines) |
| 2026-07-22 周三 | 面试前背诵 | 后端基础：HTTP/REST/Session/JWT/CORS/CSRF；AI 命理平台项目闭环；Stripe Checkout/PaymentIntent/订单状态机；等 6 项 | [HTTP](05-retrofit-okhttp-network/01-http-request-chain.md) / [支付](07-payment-engineering/01-payment-core-concepts.md) / [Django](13-backend-basics/04-django-project-defense.md) / [AI命理项目](06-resume-project-defense/02-tellyourfortune-ai.md) / [项目回答](06-resume-project-defense/03-project-three-part-answer.md) | MDN HTTP + Django docs / 项目代码/简历 |
| 2026-07-23 周四 | 面试前背诵 | 后端基础：Django 项目防线；全量八股快速复盘；项目问答稿定稿；等 6 项 | [项目回答](06-resume-project-defense/03-project-three-part-answer.md) / [支付](07-payment-engineering/01-payment-core-concepts.md) / [Django](13-backend-basics/04-django-project-defense.md) / [Activity/组件](02-android-basics/02-android-components-lifecycle.md) / [Handler/ANR](02-android-basics/03-handler-thread-anr.md) / [MVVM](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md) | Django docs / 速通目录背诵清单 |
| 2026-07-24 周五 | 首面冲刺 | Java + 后端临面速记；首面当天速记；面试后复盘；等 4 项 | [集合](12-java-basics/02-java-collections.md) / [支付](07-payment-engineering/01-payment-core-concepts.md) / [Webhook/支付回答](07-payment-engineering/02-payment-interview-order.md) / [Handler/ANR](02-android-basics/03-handler-thread-anr.md) / [Compose](04-jetpack-compose/01-compose-core-concepts.md) / [项目回答](06-resume-project-defense/03-project-three-part-answer.md) | 速通目录 12/13 章 / 个人错题本 |
| 2026-07-25 周六 | 边面边补 | Hilt/Room/Navigation/WorkManager 小闭环；性能优化基础 | [MVVM](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md) / [ViewModel/Flow](03-mvvm-jetpack-architecture/02-viewmodel-livedata-flow-stateflow.md) / [Compose](04-jetpack-compose/01-compose-core-concepts.md) / [背诵清单](10-recite-checklist/README.md) | [教程](https://developer.android.com/training/dependency-injection/hilt-android) / Android Developers |
| 2026-07-26 周日 | 边面边补 | 手写 Compose + MVVM + Retrofit demo；继续投递/约面跟进 | [MVVM](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md) / [ViewModel/Flow](03-mvvm-jetpack-architecture/02-viewmodel-livedata-flow-stateflow.md) / [Compose](04-jetpack-compose/01-compose-core-concepts.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | [教程](https://developer.android.com/codelabs/basic-android-kotlin-compose-getting-data-internet) / 招聘平台 |
| 2026-07-27 周一 | 边面边补 | Agent 基础系统化；投递 + 面试邀约跟进；后端基础：可靠性补深 | [Agent](08-agent-development/01-agent-vocabulary.md) / [MCP](08-agent-development/03-react-tooluse-harness-mcp.md) / [Agent](08-agent-development/01-agent-vocabulary.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | [教程](https://developers.openai.com/api/docs/guides/tools) / 招聘平台 |
| 2026-07-28 周二 | 边面边补 | 支付进阶：对账/退款/异常；后端可靠性话术 | [支付](07-payment-engineering/01-payment-core-concepts.md) / [后端](13-backend-basics/01-web-request-chain.md) / [JUC](12-java-basics/04-concurrency-juc-minimum-defense.md) / [Stripe](07-payment-engineering/03-stripe-payment-loop-boundary.md) / [支付](07-payment-engineering/01-payment-core-concepts.md) | [教程](https://docs.stripe.com/bank-reconciliation) / Stripe docs + Django docs |
| 2026-07-29 周三 | 边面边补 | Android 进阶：进程/IPC/Framework 概念；Hot100 高频 10 题；Java八股：JUC/类加载/AQS 扩展 | [Activity/组件](02-android-basics/02-android-components-lifecycle.md) / [算法/背诵](10-recite-checklist/01-android-high-frequency.md) | Android 面试资料 / LeetCode Hot100 |
| 2026-07-30 周四 | 边面边补 | 项目故事升级；模拟面试 4：综合版 | [项目回答](06-resume-project-defense/03-project-three-part-answer.md) / [项目回答](06-resume-project-defense/03-project-three-part-answer.md) / [支付](07-payment-engineering/01-payment-core-concepts.md) / [Agent](08-agent-development/01-agent-vocabulary.md) | 简历 / 错题本 |
| 2026-07-31 周五 | 边面边补 | Compose demo 二次完善；面试/投递复盘周报 | [MVVM](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md) / [Compose](04-jetpack-compose/01-compose-core-concepts.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | 自己的 demo / 表格记录 |
| 2026-08-01 周六 | Offer冲刺 | 错题本全量清理；目标公司二次触达 | [背诵清单](10-recite-checklist/README.md) / [项目回答](06-resume-project-defense/03-project-three-part-answer.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | 错题本 / 招聘平台 |
| 2026-08-02 周日 | Offer冲刺 | RAG/MCP/Skill 实践理解；Hot100 高频 10 题第二组 | [Agent](08-agent-development/01-agent-vocabulary.md) / [MCP](08-agent-development/03-react-tooluse-harness-mcp.md) / [算法/背诵](10-recite-checklist/01-android-high-frequency.md) | OpenAI docs / LeetCode Hot100 |
| 2026-08-03 周一 | Offer冲刺 | 支付面试深挖稿；集中面试/约面 | [Stripe](07-payment-engineering/03-stripe-payment-loop-boundary.md) / [支付](07-payment-engineering/01-payment-core-concepts.md) / [Webhook/支付回答](07-payment-engineering/02-payment-interview-order.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | Stripe docs / 招聘平台 |
| 2026-08-04 周二 | Offer冲刺 | 终轮/复面准备；安卓高频最后复盘 | [项目回答](06-resume-project-defense/03-project-three-part-answer.md) / [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) / [Activity/组件](02-android-basics/02-android-components-lifecycle.md) / [Handler/ANR](02-android-basics/03-handler-thread-anr.md) / [MVVM](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md) | 公司官网/JD / 速通目录 |
| 2026-08-05 周三 | Offer冲刺 | Offer 转化日；若未拿到 offer，调整策略 | [投递/边界](11-interview-strategy/03-project-boundary-honesty.md) | 招聘平台/HR / 投递数据 + 面试记录 |

in process:

- [ ] 逐篇补正文：先 P0 面试防线，再 P1/P2 扩展。
- [x] 已同步飞书多维表格，生成日期任务表和快捷导航。
- [ ] 推荐资料按“官方优先 -> 中文/视频辅助 -> 项目实践”补链接。

### 使用指南

- git clone 到本地后，用 Typora / VS Code 打开 Markdown 文件即可阅读和编辑。
- 每篇文章先保留标题和写作提纲占位，正文后续逐步补齐。
- 如果想调整顺序，优先改 README 和对应专栏 README，保持“专栏 -> 文章”索引同步。

---

# Map

### 目标和日期校正

- [投递方向和学习边界](00-goals-and-date/01-scope-and-learning-boundary.md)
- [7月24日前优先级](00-goals-and-date/02-before-july-24-priority.md)
- [面试速通答法约定](00-goals-and-date/03-interview-answer-convention.md)
### 总体学习顺序

- [P0到P2路线图](01-learning-order/01-p0-to-p2-roadmap.md)
- [安卓主线与Agent辅线](01-learning-order/02-android-main-agent-side-track.md)
- [每日复盘和背诵节奏](01-learning-order/03-daily-review-rhythm.md)
### Android 基础八股目录（P0）

- [Java-Kotlin最小防线](02-android-basics/01-java-kotlin-minimum-defense.md)
- [四大组件和生命周期](02-android-basics/02-android-components-lifecycle.md)
- [Handler线程ANR](02-android-basics/03-handler-thread-anr.md)
- [UI布局RecyclerView自定义View](02-android-basics/04-ui-layout-recyclerview-custom-view.md)
- [权限存储网络基础](02-android-basics/05-permission-storage-network.md)
### MVVM / Jetpack / 现代安卓架构（P0-P1）

- [MVVM最小模型](03-mvvm-jetpack-architecture/01-mvvm-minimum-model.md)
- [ViewModel-LiveData-Flow-StateFlow](03-mvvm-jetpack-architecture/02-viewmodel-livedata-flow-stateflow.md)
- [Jetpack组件速通](03-mvvm-jetpack-architecture/03-jetpack-components.md)
### Jetpack Compose 速通（P0）

- [Compose必会概念](04-jetpack-compose/01-compose-core-concepts.md)
- [Compose-MVVM标准话术](04-jetpack-compose/02-compose-mvvm-answer.md)
### Retrofit / OkHttp / 网络层（P0）

- [HTTP请求链路](05-retrofit-okhttp-network/01-http-request-chain.md)
- [Retrofit与OkHttp分工](05-retrofit-okhttp-network/02-retrofit-okhttp-roles.md)
- [拦截器错误处理和协程调用](05-retrofit-okhttp-network/03-interceptor-error-coroutine.md)
### 简历项目追问防线（P0）

- [退化场景SLAM Android客户端](06-resume-project-defense/01-slam-android-client.md)
- [TellYourFortune-AI相面命理平台](06-resume-project-defense/02-tellyourfortune-ai.md)
- [项目三段式回答模板](06-resume-project-defense/03-project-three-part-answer.md)
### 支付工程速通（P0-P1）

- [支付必会概念](07-payment-engineering/01-payment-core-concepts.md)
- [支付面试回答顺序](07-payment-engineering/02-payment-interview-order.md)
- [Stripe支付闭环和边界](07-payment-engineering/03-stripe-payment-loop-boundary.md)
### Agent 开发速通（P1-P2）

- [Agent必会词表](08-agent-development/01-agent-vocabulary.md)
- [Agent面试能讲版本](08-agent-development/02-agent-interview-version.md)
- [ReAct-ToolUse-Harness-MCP](08-agent-development/03-react-tooluse-harness-mcp.md)
### 推荐资料索引

- [官方优先](09-resources/01-official-first.md)
- [中文视频辅助](09-resources/02-chinese-video-support.md)
- [资源使用节奏](09-resources/03-resource-study-rhythm.md)
### 背诵清单

- [安卓高频题](10-recite-checklist/01-android-high-frequency.md)
- [项目高频追问](10-recite-checklist/02-project-follow-up-questions.md)
- [Java后端补位题](10-recite-checklist/03-java-backend-supplement.md)
### 面试策略

- [三段式回答](11-interview-strategy/01-three-part-answer.md)
- [不会的问题怎么收口](11-interview-strategy/02-how-to-handle-unknowns.md)
- [项目边界和诚实表达](11-interview-strategy/03-project-boundary-honesty.md)
### Java 八股速通（P0）

- [Java语言基础](12-java-basics/01-java-language-basics.md)
- [集合框架](12-java-basics/02-java-collections.md)
- [JVM-GC最小防线](12-java-basics/03-jvm-gc-minimum-defense.md)
- [并发-JUC最小防线](12-java-basics/04-concurrency-juc-minimum-defense.md)
- [Java背诵优先级](12-java-basics/05-java-recite-priority.md)
### 后端基础速通（P0-P1）

- [Web请求链路](13-backend-basics/01-web-request-chain.md)
- [数据库基础](13-backend-basics/02-database-basics.md)
- [Redis缓存最小防线](13-backend-basics/03-redis-cache-minimum-defense.md)
- [Django项目面试防线](13-backend-basics/04-django-project-defense.md)
- [支付后端和普通后端的区别](13-backend-basics/05-payment-backend-vs-general-backend.md)
- [后端背诵优先级](13-backend-basics/06-backend-recite-priority.md)

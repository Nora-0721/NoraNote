# NoraNote

面向 2026 年暑期求职的 Android 面试速通与项目追问笔记库：先在 7 月 24 日前建立首面防线，再边面边补到 8 月 5 日的 Offer 目标。

> 主投：Android 客户端｜辅投：Agent 开发｜后端：Agent、AI 命理平台和 Stripe 支付的共同工程底座

## 现在开始

- [今日与完整任务表](daily-plan.md)
- [7 月 18 日至 24 日冲刺路线](00-start-here/03-july-18-to-24-sprint.md)
- [Android P0 背诵清单](07-interview-drills/01-android-p0-recite-list.md)
- [项目追问清单](07-interview-drills/02-project-follow-up-list.md)
- [本周必用资源](08-resources/02-july-18-to-24-must-use.md)
- [错题与面试后复盘](07-interview-drills/05-mistakes-and-post-interview-review.md)

## 7 月 18 日至 24 日快捷导航

| 日期 | 阶段 | 当日主线 | 快捷 MD 笔记 | 推荐教程/资料 |
| --- | --- | --- | --- | --- |
| 2026-07-18 周六 | 投递前抢救 | 简历防线；Java/Kotlin；Activity；Handler；SLAM 数据链路 | [项目回答](03-resume-projects/01-project-answer-framework.md) / [Java/Kotlin](01-android-foundation/01-java-kotlin-minimum-pack.md) / [Activity](01-android-foundation/03-activity-lifecycle-task-stack.md) / [Handler](01-android-foundation/05-handler-looper-messagequeue.md) / [SLAM](03-resume-projects/02-slam-system-and-data-flow.md) | [Kotlin Tour](https://kotlinlang.org/docs/kotlin-tour-welcome.html) / [Activity codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-activity-lifecycle) / [Gityuan Handler](https://gityuan.com/2015/12/26/handler-message-framework/) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-18) |
| 2026-07-19 周日 | 投递前抢救 | 集合/JVM；四大组件；UI/View；MVVM；网络基础 | [集合/JVM](01-android-foundation/02-collections-jvm-concurrency.md) / [四大组件](01-android-foundation/04-fragment-and-four-components.md) / [View](01-android-foundation/07-recyclerview-custom-view-touch.md) / [MVVM](02-android-modern-stack/03-mvvm-udf-and-repository.md) / [网络](02-android-modern-stack/05-retrofit-okhttp-request-chain.md) | [JavaGuide 集合](https://javaguide.cn/java/collection/java-collection-questions-01.html) / [ViewModel codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-viewmodel-and-state) / [小林 HTTP](https://www.xiaolincoding.com/network/2_http/http_interview.html) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-19) |
| 2026-07-20 周一 | 面试前背诵 | JUC；Compose；Retrofit/OkHttp；现代 Android 数据链路；模拟面试 | [集合/JUC](01-android-foundation/02-collections-jvm-concurrency.md) / [Compose](02-android-modern-stack/04-compose-state-recomposition-effects.md) / [网络链路](02-android-modern-stack/05-retrofit-okhttp-request-chain.md) / [模拟面试](07-interview-drills/04-mock-interview-rounds.md) | [Compose Basics](https://developer.android.com/codelabs/jetpack-compose-basics) / [Retrofit](https://square.github.io/retrofit/) / [Room StateFlow](https://developer.android.com/codelabs/basic-android-kotlin-compose-update-data-room) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-20) |
| 2026-07-21 周二 | 面试前背诵 | 协程/Flow/StateFlow；SLAM 线程、渲染与内存；Jetpack 组件 | [协程](02-android-modern-stack/01-coroutines-and-structured-concurrency.md) / [Flow](02-android-modern-stack/02-flow-stateflow-and-ui-state.md) / [SLAM 性能](03-resume-projects/03-slam-thread-render-memory.md) / [Jetpack](02-android-modern-stack/06-room-navigation-hilt-workmanager.md) | [协程 codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-coroutines-kotlin-playground) / [OpenGL 环境](https://developer.android.com/develop/ui/views/graphics/opengl/environment) / [Room codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-persisting-data-room) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-21) |
| 2026-07-22 周三 | 面试前背诵 | Web/鉴权；AI 平台闭环；Stripe；Webhook；Agent 工具调用 | [Web/鉴权](04-backend-for-agent-and-payment/01-http-rest-auth-and-security.md) / [AI 平台](03-resume-projects/04-ai-platform-business-loop.md) / [Stripe](05-payment-engineering/02-stripe-checkout-paymentintent-flow.md) / [Webhook](05-payment-engineering/03-webhook-signature-and-idempotency.md) / [Tool Use](06-agent-engineering/02-tool-use-and-function-calling.md) | [Stripe Checkout](https://docs.stripe.com/payments/checkout/how-checkout-works) / [Stripe Webhooks](https://docs.stripe.com/webhooks) / [OpenAI Agent 指南](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-22) |
| 2026-07-23 周四 | 面试前背诵 | Django/数据库/异步；全量复盘；项目问答定稿；压力模拟 | [Django](04-backend-for-agent-and-payment/02-django-request-and-service-layers.md) / [数据库](04-backend-for-agent-and-payment/03-data-model-transactions-and-indexes.md) / [异步幂等](04-backend-for-agent-and-payment/05-async-jobs-retry-and-idempotency.md) / [项目追问](07-interview-drills/02-project-follow-up-list.md) / [模拟面试](07-interview-drills/04-mock-interview-rounds.md) | [Django 教程](https://docs.djangoproject.com/en/6.0/intro/tutorial01/) / [PostgreSQL 事务](https://www.postgresql.org/docs/current/tutorial-transactions.html) / [Redis](https://redis.io/docs/latest/develop/) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-23) |
| 2026-07-24 周五 | 首面冲刺 | 临面速记；项目与支付防线；面试后复盘；按反馈返工 | [P0 背诵](07-interview-drills/01-android-p0-recite-list.md) / [项目回答](03-resume-projects/01-project-answer-framework.md) / [支付防线](05-payment-engineering/06-payment-interview-defense.md) / [复盘](07-interview-drills/05-mistakes-and-post-interview-review.md) | [JavaGuide](https://javaguide.cn/home.html) / [Android P0](07-interview-drills/01-android-p0-recite-list.md) / [项目回答](03-resume-projects/01-project-answer-framework.md) / [当日完整资源](08-resources/02-july-18-to-24-must-use.md#2026-07-24) |


## 专栏地图

| 专栏 | 专栏 | 专栏 |
| --- | --- | --- |
| [从这里开始](00-start-here/README.md) | [Android 基础防线](01-android-foundation/README.md) | [Android 现代技术栈](02-android-modern-stack/README.md) |
| [简历项目防线](03-resume-projects/README.md) | [Agent 与支付所需后端](04-backend-for-agent-and-payment/README.md) | [支付工程防线](05-payment-engineering/README.md) |
| [Agent 工程速通](06-agent-engineering/README.md) | [面试训练与复盘](07-interview-drills/README.md) | [速通资源导航](08-resources/README.md) |

## 7 月 24 日后

- 按面试反馈补 [Jetpack 组件](02-android-modern-stack/06-room-navigation-hilt-workmanager.md)、[完整 Demo 地图](02-android-modern-stack/07-compose-mvvm-retrofit-demo-map.md) 和 Android 性能/Framework。
- 深化 [退款、对账与恢复](05-payment-engineering/05-refund-reconciliation-and-recovery.md)、[Agent 后端服务](06-agent-engineering/05-agent-backend-service-architecture.md) 与 [Evals/Tracing](06-agent-engineering/06-evals-tracing-and-guardrails.md)。
- 长资料统一放在 [7 月 24 日后参考资料](08-resources/06-after-july-24-reference.md)。

## GitHub 与飞书分工

- GitHub：稳定文章路径、长期笔记和资源说明的主版本。
- 飞书多维表格：日程、完成状态和临时调整。
- 飞书资源推荐：手机端快捷入口，并链接回 GitHub 对应文章。
- [速通目录计划文档](https://gcnbv9droju6.feishu.cn/wiki/Kh7lw79U5if5rekNGLGcVSMPnFe) · [多维表格](https://gcnbv9droju6.feishu.cn/wiki/Vq2gwpGSaibpF3kfKy8chSiDnid) · [资源推荐](https://gcnbv9droju6.feishu.cn/wiki/HNGpwb66Xi3wOmk4Xdacy39onng)

## 使用方式

1. 先从当天一行进入对应的空壳 MD。
2. 按必用资源学习，把自己的理解写进空壳。
3. 用 30 秒和 2 分钟版本口述，再去背诵清单打勾。
4. 面试后只在复盘页记录错题，再回到唯一文章补内容。

## 同行寄语

> 2026-07-19 · [@Link-wushuang](https://github.com/Link-wushuang) 说：lcf 加油，一起上岸。

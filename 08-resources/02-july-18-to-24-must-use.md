# 7 月 18 日至 24 日必用资源

> 只把 1–2 个资源标为必看。建议范围之外先不展开；个人简历、项目代码和错题本也是项目类任务的一手资料。
>
> 本页已对照"速通安卓邪修"33 道真实面试题补齐 Kotlin 专题、Service、BroadcastReceiver、布局优化、设计模式、JSON、内存泄漏、数据结构算法等缺口；邪修逐题答案见 [速通邪修八股答案与教程](./07-速通邪修八股答案与教程.md)。

## 2026-07-18

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D01-1` 简历防线 | [项目回答](../03-resume-projects/01-project-answer-framework.md) | 个人简历 + [30 秒与 2 分钟回答法](../00-start-here/04-thirty-second-two-minute-answer.md) | 只整理两段项目经历 / 60 分钟 | 直接对应本人经历 | 两段 2 分钟回答 | 一手 |
| `D01-2` Java/Kotlin 最小包 | [Java/Kotlin](../01-android-foundation/01-java-kotlin-minimum-pack.md) | [Kotlin Tour](https://kotlinlang.org/docs/kotlin-tour-welcome.html) / [JavaGuide 基础](https://javaguide.cn/java/basis/java-basic-questions-01.html) | Tour 的 null safety、classes、collections；JavaGuide 只看高频问答 / 90 分钟 | 官方交互式入门 + 156K+ Star 中文面试库 | 语言差异口述 | 官方 + 高口碑 |
| `D01-3` Activity | [Activity](../01-android-foundation/03-activity-lifecycle-task-stack.md) | [Activity 生命周期 codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-activity-lifecycle) / [任务与返回栈](https://developer.android.com/guide/components/activities/tasks-and-back-stack) | codelab 1–6 节；返回栈只看概览和 launch modes / 75 分钟 | 有成品、Logcat 实验和场景图 | 生命周期场景图 | Android 官方 |
| `D01-4` Handler/ANR | [Handler](../01-android-foundation/05-handler-looper-messagequeue.md) | [Gityuan Handler 消息机制](https://gityuan.com/2015/12/26/handler-message-framework/) / [Android 线程与主线程](https://developer.android.com/develop/background-work/background-tasks/asynchronous/java-threads) | Gityuan 看 Java 层流程图；官方文档看主线程规则 / 70 分钟 | 经典中文源码图解 + 官方边界 | 消息循环图与 ANR 原因 | 高口碑 + 官方 |
| `D01-5` SLAM 故事线 | [SLAM 数据流](../03-resume-projects/02-slam-system-and-data-flow.md) | 项目代码/简历 + [Android OpenGL 环境](https://developer.android.com/develop/ui/views/graphics/opengl/environment) | 先画本人链路；官方只看 GLSurfaceView 与 Renderer / 90 分钟 | 项目证据优先，官方补渲染线程术语 | 三端链路图 | 一手 + 官方 |
| `D01-J1` Java 语言基础 | [集合/JVM](../01-android-foundation/02-collections-jvm-concurrency.md) | [JavaGuide 基础](https://javaguide.cn/java/basis/java-basic-questions-01.html) | 面向对象、异常、泛型、反射 / 60 分钟 | 题目集中、中文回答短 | 10 题口述 | 高口碑 |
| `D01-J2` 设计模式 | [集合/JVM](../01-android-foundation/02-collections-jvm-concurrency.md) | [Java 23 种设计模式全归纳](https://cloud.tencent.com/developer/article/1602270) / [一文速通 23 种设计模式](http://blog.mvui.cn/index.php/detail/106170.html) | 单例、工厂、观察者、责任链、建造者 / 45 分钟 | 邪修高频追问；Android 中常见 | 5 个模式口述 | 高口碑 |
| `D01-K1` Kotlin 专题 | [Java/Kotlin](../01-android-foundation/01-java-kotlin-minimum-pack.md) | [Kotlin 作用域函数对比](https://juejin.cn/post/7504846684335947788) / [inline/reified 隐藏开销](https://juejin.cn/post/7640789716057554953) | 高阶函数、挂起函数、let/run/with/apply/also、与 Java 区别 / 60 分钟 | 邪修明确点名；面试只问这些 | 5 函数区别表 | 高口碑 |

核验日期：2026-07-18。

## 2026-07-19

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D02-J1` 集合与 HashMap | [集合/JVM](../01-android-foundation/02-collections-jvm-concurrency.md) | [JavaGuide 集合面试题](https://javaguide.cn/java/collection/java-collection-questions-01.html) / [HashMap 源码分析](https://javaguide.cn/java/collection/hashmap-source-code.html) | ArrayList、HashMap、ConcurrentHashMap / 75 分钟 | 热度高且按面试问题组织 | 集合对比与 HashMap 口述 | 高口碑 |
| `D02-1` 组件/权限/存储 | [四大组件](../01-android-foundation/04-fragment-and-four-components.md) / [权限存储](../01-android-foundation/08-permissions-storage-and-process.md) | [应用基础与组件](https://developer.android.com/guide/components/fundamentals) / [数据与文件存储](https://developer.android.com/training/data-storage) | 组件概览；存储只看分类和 scoped storage / 75 分钟 | 官方一页建立边界 | 组件对比表 | Android 官方 |
| `D02-2` RecyclerView/View | [View 与事件](../01-android-foundation/07-recyclerview-custom-view-touch.md) | [RecyclerView 动态列表](https://developer.android.com/develop/ui/views/layout/recyclerview) / [自定义绘制](https://developer.android.com/develop/ui/views/layout/custom-views/custom-drawing) | Adapter/ViewHolder；onDraw 与尺寸 / 75 分钟 | 示例和结构图完整 | 复用、绘制、事件三段口述 | Android 官方 |
| `D02-3` MVVM/ViewModel | [MVVM](../02-android-modern-stack/03-mvvm-udf-and-repository.md) | [ViewModel 与 State codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-viewmodel-and-state) / [应用架构指南](https://developer.android.com/topic/architecture) | codelab 4–7 节；架构指南只看 UI/Data layer 图 / 90 分钟 | 有完整应用和架构图 | MVVM 分层图 | Android 官方 |
| `D02-4` HTTP/HTTPS/TCP | [Web/鉴权](../04-backend-for-agent-and-payment/01-http-rest-auth-and-security.md) | [小林 HTTP 面试题](https://www.xiaolincoding.com/network/2_http/http_interview.html) / [小林 TCP 面试题](https://xiaolincoding.com/network/3_tcp/tcp_interview.html) | HTTP/HTTPS 与握手挥手 / 75 分钟 | 图多、讲解生动、面试口碑稳定 | HTTP/TLS/TCP 口述 | 高口碑 |
| `D02-5` 自我介绍录音 | [回答法](../00-start-here/04-thirty-second-two-minute-answer.md) | 个人简历 + 手机录音 | 录三遍并回听 / 60 分钟 | 本人输出比继续看教程有效 | 1 分钟自我介绍 + 2 分钟项目 | 一手 |
| `D02-J2` JVM/GC | [集合/JVM](../01-android-foundation/02-collections-jvm-concurrency.md) | [JavaGuide JVM 垃圾回收](https://javaguide.cn/java/jvm/jvm-garbage-collection.html) / [Android 内存管理概览](https://developer.android.com/topic/performance/memory-overview) | GC Roots、可达性、泄漏边界 / 60 分钟 | 面试问答 + Android 场景 | JVM/GC 与泄漏口述 | 高口碑 + 官方 |
| `D02-6` 内存泄漏专项 | [Handler](../01-android-foundation/05-handler-looper-messagequeue.md) / [线程与内存](../01-android-foundation/06-threading-anr-and-memory-leaks.md) | [LeakCanary 原理与定制](https://www.cnblogs.com/dblens/p/19554504) / [LeakCanary 面试考点](https://knowledge.meng-github.com/00-android/13_Testing/08_%E5%86%85%E5%AD%98%E6%B3%84%E6%BC%8F_LeakCanary.html) | 常见泄漏场景、检测原理、修复 / 45 分钟 | 邪修 Handler 追问直接问泄漏 | 泄漏场景清单 | 高口碑 |
| `D02-7` JSON 解析 | [网络链路](../02-android-modern-stack/05-retrofit-okhttp-request-chain.md) | [Gson 与 Moshi 对比](https://blog.csdn.net/2600_94959881/article/details/157318412) / [从 Gson 迁移到 Moshi](https://icode.best/i/758747421214361) | Gson/Moshi 选型、data class 解析 / 30 分钟 | 邪修第 9 题；网络链路配套 | JSON 解析口述 | 高口碑 |

核验日期：2026-07-18。

## 2026-07-20

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D03-J1` JUC | [集合/JVM](../01-android-foundation/02-collections-jvm-concurrency.md) | [JavaGuide 并发面试题](https://javaguide.cn/java/concurrent/java-concurrent-questions-01.html) / [Oracle 并发教程](https://docs.oracle.com/javase/tutorial/essential/concurrency/) | synchronized、volatile、线程池 / 75 分钟 | 中文面试入口 + 官方定义 | 并发三要素口述 | 高口碑 + 官方 |
| `D03-1` 岗位 JD | [职责边界](../03-resume-projects/06-truth-boundaries-and-metrics.md) | 招聘平台的真实 JD | 记录 10 个重复关键词 / 45 分钟 | 直接校正优先级 | JD 高频词表 | 一手 |
| `D03-2` Compose | [Compose](../02-android-modern-stack/04-compose-state-recomposition-effects.md) | [Compose Basics codelab](https://developer.android.com/codelabs/jetpack-compose-basics) / [Compose State codelab](https://developer.android.com/codelabs/jetpack-compose-state) | Basics 1–5；State 看 state hoisting / 90 分钟 | 有成品、动画和状态示例 | 状态上提图 | Android 官方 |
| `D03-3` Retrofit/OkHttp | [网络链路](../02-android-modern-stack/05-retrofit-okhttp-request-chain.md) | [Retrofit 官方教程](https://square.github.io/retrofit/) / [OkHttp Interceptors](https://square.github.io/okhttp/features/interceptors/) | Retrofit 声明接口；拦截器链 / 75 分钟 | 一手、示例短、可直接对应项目 | 请求链路图 | Square 官方 |
| `D03-4` Compose + StateFlow | [Flow](../02-android-modern-stack/02-flow-stateflow-and-ui-state.md) | [ViewModel 与 State codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-viewmodel-and-state) / [Room 中使用 StateFlow](https://developer.android.com/codelabs/basic-android-kotlin-compose-update-data-room) | 只看 UiState、StateFlow、collect 部分 / 75 分钟 | 一条链路展示状态如何到 UI | 标准数据流图 | Android 官方 |
| `D03-5` 模拟面试 1 | [模拟面试](../07-interview-drills/04-mock-interview-rounds.md) | [Android P0 清单](../07-interview-drills/01-android-p0-recite-list.md) + 手机录音 | 40 分钟问答 + 20 分钟复盘 | 强制输出 | 评分表与错题 | 自测 |
| `D03-6` Service | [四大组件](../01-android-foundation/04-fragment-and-four-components.md) | [Service 面试题干货](https://developer.aliyun.com/article/928972) / [Service 生命周期](https://cloud.tencent.com/developer/article/2531026) | startService/bindService 生命周期、Activity vs Service / 45 分钟 | 邪修第 30/31/33 题；must-use 原缺 | 启动方式对比表 | 高口碑 |
| `D03-7` BroadcastReceiver | [四大组件](../01-android-foundation/04-fragment-and-four-components.md) | [BroadcastReceiver 面试题](https://cloud.tencent.com/developer/article/2531027) / [Broadcast 使用与实例](https://developer.aliyun.com/article/929298) | 静态/动态注册、有序/标准广播、耗时处理 / 45 分钟 | 邪修第 32/33 题；must-use 原缺 | 注册方式对比表 | 高口碑 |

核验日期：2026-07-18。

## 2026-07-21

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D04-J1` Java 口述 | [集合/JVM](../01-android-foundation/02-collections-jvm-concurrency.md) | 前三日错题本 | 只测未通过题 / 60 分钟 | 防止重复阅读 | 未通过清单 | 自测 |
| `D04-1` 协程/Flow | [协程](../02-android-modern-stack/01-coroutines-and-structured-concurrency.md) / [Flow](../02-android-modern-stack/02-flow-stateflow-and-ui-state.md) | [协程 Playground codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-coroutines-kotlin-playground) / [Android 协程指南](https://developer.android.com/kotlin/coroutines) | structured concurrency、取消、dispatcher / 90 分钟 | 交互式练习 + 官方 Android 边界 | 取消与异常传播图 | Android 官方 |
| `D04-2` SLAM 深挖 | [SLAM 性能](../03-resume-projects/03-slam-thread-render-memory.md) | 项目代码/Profiler 截图 + [OpenGL 环境](https://developer.android.com/develop/ui/views/graphics/opengl/environment) | 线程、Renderer、buffer 复用 / 120 分钟 | 本人证据优先 | 线程图和指标证据 | 一手 + 官方 |
| `D04-3` Jetpack 组件 | [Jetpack](../02-android-modern-stack/06-room-navigation-hilt-workmanager.md) | [Room codelab](https://developer.android.com/codelabs/basic-android-kotlin-compose-persisting-data-room) / [WorkManager 指南](https://developer.android.com/develop/background-work/background-tasks/persistent/getting-started) | 每个组件只回答“解决什么” / 60 分钟 | 有实际代码，又能控制深度 | 组件选择表 | Android 官方 |
| `D04-4` 模拟面试 2 | [项目追问](../07-interview-drills/02-project-follow-up-list.md) | 个人简历 + 项目代码 + 手机录音 | 45 分钟问答 / 60 分钟 | 项目题必须回到真实证据 | 项目错题清单 | 一手 |
| `D04-5` 布局优化 | [View 与事件](../01-android-foundation/07-recyclerview-custom-view-touch.md) | [ConstraintLayout 性能提升](https://blog.csdn.net/kkshdgxcjsd/article/details/154289307) / [CoordinatorLayout 基本使用](https://juejin.cn/post/7548278406836879401) | 减少嵌套、ConstraintLayout、CoordinatorLayout / 45 分钟 | 邪修第 9/10 题；must-use 原缺 | 布局优化口述 | 高口碑 |

核验日期：2026-07-18。

## 2026-07-22

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D05-B1` HTTP/鉴权 | [Web/鉴权](../04-backend-for-agent-and-payment/01-http-rest-auth-and-security.md) | [MDN HTTP Overview](https://developer.mozilla.org/en-US/docs/Web/HTTP/Guides/Overview) / [Django Auth](https://docs.djangoproject.com/en/6.0/topics/auth/) | 请求/响应、Session、权限 / 75 分钟 | Web 标准解释 + 框架落点 | 请求与鉴权链路 | MDN + Django 官方 |
| `D05-1` AI 平台闭环 | [AI 平台](../03-resume-projects/04-ai-platform-business-loop.md) | 项目代码/简历 + [AI 输出与成本空壳](../03-resume-projects/05-ai-output-persistence-and-cost.md) | 只沿本人业务链路复盘 / 90 分钟 | 防止被泛化 Agent 教程带偏 | 业务闭环图 | 一手 |
| `D05-2` Stripe | [Stripe 链路](../05-payment-engineering/02-stripe-checkout-paymentintent-flow.md) | [Checkout 生命周期](https://docs.stripe.com/payments/checkout/how-checkout-works) / [PaymentIntents](https://docs.stripe.com/payments/payment-intents) | hosted checkout 与 PaymentIntent 状态 / 90 分钟 | 官方可操作流程和生命周期 | 支付时序图 | Stripe 官方 |
| `D05-3` Webhook/幂等 | [Webhook](../05-payment-engineering/03-webhook-signature-and-idempotency.md) | [Stripe Webhooks](https://docs.stripe.com/webhooks) / [Idempotent Requests](https://docs.stripe.com/api/idempotent_requests) | handler、验签、快速 2xx、重复事件 / 75 分钟 | 官方明确安全和重试边界 | Webhook 消费流程 | Stripe 官方 |
| `D05-4` Agent 入门 | [Agent 循环](../06-agent-engineering/01-agent-workflow-and-agent-loop.md) | [OpenAI 实用 Agent 指南](https://openai.com/business/guides-and-resources/a-practical-guide-to-building-ai-agents/) / [MCP 架构](https://modelcontextprotocol.io/docs/learn/architecture) | 先看 Agent 定义、工具、循环；再看 MCP primitives / 75 分钟 | 生动、广受引用、工程边界清晰 | Agent 循环图 | OpenAI + MCP 官方 |
| `D05-B2` 事务/索引 | [数据库](../04-backend-for-agent-and-payment/03-data-model-transactions-and-indexes.md) | [PostgreSQL Transactions](https://www.postgresql.org/docs/current/tutorial-transactions.html) / [PostgreSQL Indexes](https://www.postgresql.org/docs/current/indexes.html) | 事务原子性、唯一约束、B-tree / 75 分钟 | 短且权威 | 订单更新事务口述 | PostgreSQL 官方 |
| `D05-B3` HTTP 状态码/HTTPS | [Web/鉴权](../04-backend-for-agent-and-payment/01-http-rest-auth-and-security.md) | [SSL/TLS 完整握手图解](https://blog.csdn.net/qq_41840843/article/details/159994308) / [小林 HTTP 状态码](https://www.xiaolincoding.com/network/2_http/http_interview.html) | 常见状态码、TLS 四次握手、对称+非对称 / 45 分钟 | 邪修第 22/23 题；补强小林 | 状态码与握手图 | 高口碑 |

核验日期：2026-07-18。

## 2026-07-23

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D06-B1` Django | [Django](../04-backend-for-agent-and-payment/02-django-request-and-service-layers.md) | [Django 官方教程 1](https://docs.djangoproject.com/en/6.0/intro/tutorial01/) / [Request/Response](https://docs.djangoproject.com/en/6.0/ref/request-response/) | 项目结构、URL、View、request/response / 75 分钟 | 直接对应本人项目 | Django 请求链路 | Django 官方 |
| `D06-1` 全量复盘 | [Android P0](../07-interview-drills/01-android-p0-recite-list.md) | 本页前六日资源 + 个人错题本 | 只看笔记和未通过题 / 120 分钟 | 避免考前重新开新资料 | 全量未通过清单 | 自测 |
| `D06-2` 项目定稿 | [项目回答](../03-resume-projects/01-project-answer-framework.md) | 个人简历、项目代码、前日录音 | 每个项目录一版 / 90 分钟 | 真实、可验证 | 两段最终项目稿 | 一手 |
| `D06-3` 压力模拟 | [模拟面试](../07-interview-drills/04-mock-interview-rounds.md) | [项目追问](../07-interview-drills/02-project-follow-up-list.md) / [综合追问](../07-interview-drills/03-backend-payment-agent-list.md) | 连续 45 分钟 / 60 分钟 | 验证临场检索能力 | 压力版评分表 | 自测 |
| `D06-4` 算法 | [Android P0](../07-interview-drills/01-android-p0-recite-list.md) | [LeetCode Hot 100](https://leetcode.cn/studyplan/top-100-liked/) | 数组、链表、哈希各 1–2 题 / 75 分钟 | 热度高、题单稳定 | 5 题和错题原因 | 高口碑 |
| `D06-B2` Redis/异步 | [Redis](../04-backend-for-agent-and-payment/04-redis-cache-and-consistency.md) / [异步幂等](../04-backend-for-agent-and-payment/05-async-jobs-retry-and-idempotency.md) | [Redis 开发指南](https://redis.io/docs/latest/develop/) / [Celery First Steps](https://docs.celeryq.dev/en/stable/getting-started/first-steps-with-celery.html) | 缓存用途、任务队列、重试 / 75 分钟 | 对应 AI 任务和支付通知 | 缓存与异步口述 | Redis + Celery 官方 |
| `D06-5` 数据结构与算法 | [Android P0](../07-interview-drills/01-android-p0-recite-list.md) | [二叉树遍历总结](https://zhuanlan.zhihu.com/p/345762224) / [栈与队列实战](https://www.cnblogs.com/yangykaifa/p/19746831) | 数组链表、判环、栈实现队列、二叉树前后中序层序 / 60 分钟 | 邪修第 25-29 题；分类题解更高效 | 5 类题型口述 | 高口碑 |

核验日期：2026-07-18。

## 2026-07-24

| 任务 | 笔记空壳 | 必看资源 | 建议范围 / 用时 | 为什么选 | 看完产物 | 来源 |
| --- | --- | --- | --- | --- | --- | --- |
| `D07-B1` Java + 后端速记 | [综合追问](../07-interview-drills/03-backend-payment-agent-list.md) | 个人错题本 + [JavaGuide 面试主线](https://javaguide.cn/home.html) | 只查未通过题 / 30 分钟 | 不再引入新体系 | 临面卡片 | 自测 + 高口碑 |
| `D07-1` 首面当天 | [Android P0](../07-interview-drills/01-android-p0-recite-list.md) | 个人错题本 + [项目回答](../03-resume-projects/01-project-answer-framework.md) | 只读自己的答案 / 30 分钟 | 降低临面认知负担 | 最终口述 | 自测 |
| `D07-2` 面试后复盘 | [复盘](../07-interview-drills/05-mistakes-and-post-interview-review.md) | 面试记录 | 结束后立即记录 / 30 分钟 | 保留原问题和反馈 | 错题与证据缺口 | 一手 |
| `D07-3` 按反馈补洞 | [复盘](../07-interview-drills/05-mistakes-and-post-interview-review.md) | 从本页按错题回到唯一资源 | 只修首面暴露点 / 120 分钟 | 面试反馈优先于预设路线 | 返工后的 30 秒回答 | 自测 |

核验日期：2026-07-18。

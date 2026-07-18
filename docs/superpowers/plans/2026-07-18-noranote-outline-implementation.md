# NoraNote Outline Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Replace the current fragmented outline with the approved interview-first directory, complete daily navigation, and a verified resource system without writing article bodies.

**Architecture:** GitHub is the canonical store for stable article paths and resource annotations. The root README provides a five-column daily summary plus a column map; `daily-plan.md` holds task-level execution data; resource pages provide date-based and topic-based views over the same links. Feishu receives a copy-ready sync package because this environment has read access but no write connector.

**Tech Stack:** Markdown, Git, PowerShell standard library; no new dependencies or generated site.

## Global Constraints

- Hard deadlines: Android P0 defense by 2026-07-24 and first Offer target by 2026-08-05.
- Android is the primary track; Agent development is the secondary application track.
- Backend exists only as the common engineering base for Agent roles, the AI platform, and Stripe payment defense.
- Create directory shells, metadata, navigation, and resource annotations only; do not write technical article bodies.
- Preserve the README daily table columns exactly: 日期、阶段、当日主线、快捷 MD 笔记、推荐教程/资料.
- Preserve note-taking shells and link each scheduled task to one canonical article.
- Each README date row exposes 2–4 direct must-use resources plus one complete daily-resource anchor.
- Every independent P0 task has at least one must-use resource; visuals are preferred, not mandatory when a vivid, well-reviewed, popular speed-run resource is better.
- Keep one or two must-use resources per task; move remaining links to supplemental or post-2026-07-24 sections.
- Use exact links, not search phrases, author profiles, or generic homepages.
- Do not add link-checking dependencies or repository automation; use PowerShell and manual web verification.
- Do not push until all local-link, coverage, and repository-state checks pass.

---

### Task 1: Build the canonical article skeleton

**Files:**
- Create: `00-start-here/README.md`
- Create: `00-start-here/01-target-roles-and-boundaries.md`
- Create: `00-start-here/02-p0-p1-p2-priority-map.md`
- Create: `00-start-here/03-july-18-to-24-sprint.md`
- Create: `00-start-here/04-thirty-second-two-minute-answer.md`
- Create: `01-android-foundation/README.md`
- Create: `01-android-foundation/01-java-kotlin-minimum-pack.md`
- Create: `01-android-foundation/02-collections-jvm-concurrency.md`
- Create: `01-android-foundation/03-activity-lifecycle-task-stack.md`
- Create: `01-android-foundation/04-fragment-and-four-components.md`
- Create: `01-android-foundation/05-handler-looper-messagequeue.md`
- Create: `01-android-foundation/06-threading-anr-and-memory-leaks.md`
- Create: `01-android-foundation/07-recyclerview-custom-view-touch.md`
- Create: `01-android-foundation/08-permissions-storage-and-process.md`
- Create: `02-android-modern-stack/README.md`
- Create: `02-android-modern-stack/01-coroutines-and-structured-concurrency.md`
- Create: `02-android-modern-stack/02-flow-stateflow-and-ui-state.md`
- Create: `02-android-modern-stack/03-mvvm-udf-and-repository.md`
- Create: `02-android-modern-stack/04-compose-state-recomposition-effects.md`
- Create: `02-android-modern-stack/05-retrofit-okhttp-request-chain.md`
- Create: `02-android-modern-stack/06-room-navigation-hilt-workmanager.md`
- Create: `02-android-modern-stack/07-compose-mvvm-retrofit-demo-map.md`
- Create: `03-resume-projects/README.md`
- Create: `03-resume-projects/01-project-answer-framework.md`
- Create: `03-resume-projects/02-slam-system-and-data-flow.md`
- Create: `03-resume-projects/03-slam-thread-render-memory.md`
- Create: `03-resume-projects/04-ai-platform-business-loop.md`
- Create: `03-resume-projects/05-ai-output-persistence-and-cost.md`
- Create: `03-resume-projects/06-truth-boundaries-and-metrics.md`
- Create: `04-backend-for-agent-and-payment/README.md`
- Create: `04-backend-for-agent-and-payment/01-http-rest-auth-and-security.md`
- Create: `04-backend-for-agent-and-payment/02-django-request-and-service-layers.md`
- Create: `04-backend-for-agent-and-payment/03-data-model-transactions-and-indexes.md`
- Create: `04-backend-for-agent-and-payment/04-redis-cache-and-consistency.md`
- Create: `04-backend-for-agent-and-payment/05-async-jobs-retry-and-idempotency.md`
- Create: `04-backend-for-agent-and-payment/06-logging-tracing-deployment.md`
- Create: `05-payment-engineering/README.md`
- Create: `05-payment-engineering/01-order-payment-and-ledger-models.md`
- Create: `05-payment-engineering/02-stripe-checkout-paymentintent-flow.md`
- Create: `05-payment-engineering/03-webhook-signature-and-idempotency.md`
- Create: `05-payment-engineering/04-payment-state-machine-and-transactions.md`
- Create: `05-payment-engineering/05-refund-reconciliation-and-recovery.md`
- Create: `05-payment-engineering/06-payment-interview-defense.md`
- Create: `06-agent-engineering/README.md`
- Create: `06-agent-engineering/01-agent-workflow-and-agent-loop.md`
- Create: `06-agent-engineering/02-tool-use-and-function-calling.md`
- Create: `06-agent-engineering/03-mcp-resources-tools-and-prompts.md`
- Create: `06-agent-engineering/04-rag-context-and-memory.md`
- Create: `06-agent-engineering/05-agent-backend-service-architecture.md`
- Create: `06-agent-engineering/06-evals-tracing-and-guardrails.md`
- Create: `06-agent-engineering/07-agent-interview-defense.md`
- Create: `07-interview-drills/README.md`
- Create: `07-interview-drills/01-android-p0-recite-list.md`
- Create: `07-interview-drills/02-project-follow-up-list.md`
- Create: `07-interview-drills/03-backend-payment-agent-list.md`
- Create: `07-interview-drills/04-mock-interview-rounds.md`
- Create: `07-interview-drills/05-mistakes-and-post-interview-review.md`
- Create: `08-resources/README.md`
- Create: `08-resources/01-resource-selection-rules.md`
- Create: `08-resources/02-july-18-to-24-must-use.md`
- Create: `08-resources/03-android-learning-path.md`
- Create: `08-resources/04-project-backend-payment-path.md`
- Create: `08-resources/05-agent-learning-path.md`
- Create: `08-resources/06-after-july-24-reference.md`
- Modify: `article-template.md`

**Interfaces:**
- Consumes: The exact paths and boundaries in `docs/superpowers/specs/2026-07-18-noranote-outline-design.md`.
- Produces: Stable canonical article paths consumed by every later navigation and resource task.

- [ ] **Step 1: Record the pre-migration path failure**

Run:

```powershell
$required = @(
  '00-start-here/01-target-roles-and-boundaries.md',
  '01-android-foundation/03-activity-lifecycle-task-stack.md',
  '02-android-modern-stack/04-compose-state-recomposition-effects.md',
  '03-resume-projects/02-slam-system-and-data-flow.md',
  '04-backend-for-agent-and-payment/05-async-jobs-retry-and-idempotency.md',
  '05-payment-engineering/03-webhook-signature-and-idempotency.md',
  '06-agent-engineering/02-tool-use-and-function-calling.md',
  '07-interview-drills/01-android-p0-recite-list.md',
  '08-resources/02-july-18-to-24-must-use.md'
)
($required | Where-Object { -not (Test-Path $_) }).Count
```

Expected before implementation: `9`.

- [ ] **Step 2: Create directories, README files, and article shells with `apply_patch`**

Every article shell must use this exact structure with its real values filled from the approved directory:

```markdown
# Activity 生命周期与任务栈

> 优先级：P0
>
> 预计用时：45 分钟
>
> 状态：正文待写

## 预期产物

- 30 秒口述
- 生命周期与任务栈场景图
- 高频追问清单
```

Use P0 for 7/18–7/23 Android fundamentals, modern-stack essentials, resume defense, and payment safety basics. Use P1 for Jetpack supplements, backend depth, and Agent engineering basics. Use P2 only for post-7/24 depth such as full eval systems or extended reconciliation.

- [ ] **Step 3: Update the reusable article template**

Set `article-template.md` to the same metadata shape, followed by empty headings for `预期产物`, `核心概念`, `项目落点`, `坑与权衡`, and `面试回答`. Mark all body sections as `正文待写` without technical content.

- [ ] **Step 4: Verify canonical paths and shell-only scope**

Run:

```powershell
$missing = $required | Where-Object { -not (Test-Path $_) }
"MISSING_REQUIRED_PATHS=$($missing.Count)"
$bad = Get-ChildItem 00-start-here,01-android-foundation,02-android-modern-stack,03-resume-projects,04-backend-for-agent-and-payment,05-payment-engineering,06-agent-engineering,07-interview-drills -Recurse -Filter *.md |
  Where-Object { $_.Name -ne 'README.md' -and (Get-Content $_.FullName -Raw -Encoding utf8) -notmatch '状态：正文待写' }
"SHELLS_WITHOUT_STATUS=$($bad.Count)"
```

Expected: `MISSING_REQUIRED_PATHS=0` and `SHELLS_WITHOUT_STATUS=0`.

- [ ] **Step 5: Commit the canonical skeleton**

```powershell
git add article-template.md 00-start-here 01-android-foundation 02-android-modern-stack 03-resume-projects 04-backend-for-agent-and-payment 05-payment-engineering 06-agent-engineering 07-interview-drills 08-resources
git commit -m "docs: scaffold interview-first note structure"
```

---

### Task 2: Build root and column navigation

**Files:**
- Modify: `README.md`
- Modify: `00-start-here/README.md`
- Modify: `01-android-foundation/README.md`
- Modify: `02-android-modern-stack/README.md`
- Modify: `03-resume-projects/README.md`
- Modify: `04-backend-for-agent-and-payment/README.md`
- Modify: `05-payment-engineering/README.md`
- Modify: `06-agent-engineering/README.md`
- Modify: `07-interview-drills/README.md`
- Modify: `08-resources/README.md`

**Interfaces:**
- Consumes: Canonical article paths from Task 1.
- Produces: Root and per-column navigation consumed by the daily plan and public readers.

- [ ] **Step 1: Capture current root-navigation mismatches**

Run:

```powershell
$root = Get-Content README.md -Raw -Encoding utf8
"HAS_NEW_START_HERE=$($root.Contains('00-start-here/README.md'))"
"HAS_OLD_ANDROID_PATH=$($root.Contains('02-android-basics/README.md'))"
```

Expected before implementation: `HAS_NEW_START_HERE=False`, `HAS_OLD_ANDROID_PATH=True`.

- [ ] **Step 2: Rewrite the root README in the approved order**

Include: one-sentence positioning; hard deadlines; `现在开始` links; the exact five-column 7/18–7/24 table; the nine-column map rendered as a compact Markdown table; post-7/24 route; Feishu/GitHub responsibilities; and usage instructions. Keep the full task table out of README.

- [ ] **Step 3: Populate every column README with the standard table**

Use exactly:

```markdown
| 优先级 | 文章 | 预计用时 | 学完产物 | 状态 |
| --- | --- | ---: | --- | --- |
```

Each row links to one article from Task 1. Do not add topic explanations below the table.

- [ ] **Step 4: Verify all canonical articles appear once in a column README**

Run:

```powershell
$roots = '00-start-here','01-android-foundation','02-android-modern-stack','03-resume-projects','04-backend-for-agent-and-payment','05-payment-engineering','06-agent-engineering','07-interview-drills','08-resources'
$bad = foreach ($root in $roots) {
  $readme = Get-Content (Join-Path $root 'README.md') -Raw -Encoding utf8
  Get-ChildItem $root -Filter *.md | Where-Object Name -ne 'README.md' | ForEach-Object {
    $needle = './' + $_.Name
    $count = ([regex]::Matches($readme, [regex]::Escape($needle))).Count
    if ($count -ne 1) { "$($_.FullName):$count" }
  }
}
"COLUMN_LINK_COUNT_ERRORS=$($bad.Count)"
```

Expected: `COLUMN_LINK_COUNT_ERRORS=0`.

- [ ] **Step 5: Commit navigation**

```powershell
git add README.md 00-start-here/README.md 01-android-foundation/README.md 02-android-modern-stack/README.md 03-resume-projects/README.md 04-backend-for-agent-and-payment/README.md 05-payment-engineering/README.md 06-agent-engineering/README.md 07-interview-drills/README.md 08-resources/README.md
git commit -m "docs: add sprint and column navigation"
```

---

### Task 3: Remap the execution schedule

**Files:**
- Modify: `daily-plan.md`
- Modify: `README.md`
- Modify: `00-start-here/03-july-18-to-24-sprint.md`

**Interfaces:**
- Consumes: Canonical article paths from Task 1 and root navigation from Task 2.
- Produces: One task-level schedule and one date-level summary that resource pages can target by task ID and date anchor.

- [ ] **Step 1: Preserve the existing dates and task IDs**

Extract every current `daily-plan.md` date and backticked task ID before editing. Expected coverage: 2026-07-18 through 2026-08-05 with no date removed.

- [ ] **Step 2: Replace every old article link with one canonical path**

Use this mapping for all matching task rows:

| Task topic | Canonical article |
| --- | --- |
| Java/Kotlin minimum pack | `01-android-foundation/01-java-kotlin-minimum-pack.md` |
| Collections, JVM, GC, JUC | `01-android-foundation/02-collections-jvm-concurrency.md` |
| Activity lifecycle and launch modes | `01-android-foundation/03-activity-lifecycle-task-stack.md` |
| Four components and Fragment | `01-android-foundation/04-fragment-and-four-components.md` |
| Handler/Looper | `01-android-foundation/05-handler-looper-messagequeue.md` |
| Threads, ANR, leaks | `01-android-foundation/06-threading-anr-and-memory-leaks.md` |
| RecyclerView, custom View, touch | `01-android-foundation/07-recyclerview-custom-view-touch.md` |
| Permissions, storage, process | `01-android-foundation/08-permissions-storage-and-process.md` |
| Coroutines | `02-android-modern-stack/01-coroutines-and-structured-concurrency.md` |
| Flow/StateFlow | `02-android-modern-stack/02-flow-stateflow-and-ui-state.md` |
| MVVM/ViewModel/Repository | `02-android-modern-stack/03-mvvm-udf-and-repository.md` |
| Compose | `02-android-modern-stack/04-compose-state-recomposition-effects.md` |
| HTTP/Retrofit/OkHttp | `02-android-modern-stack/05-retrofit-okhttp-request-chain.md` |
| Room/Navigation/Hilt/WorkManager | `02-android-modern-stack/06-room-navigation-hilt-workmanager.md` |
| Integrated demo | `02-android-modern-stack/07-compose-mvvm-retrofit-demo-map.md` |
| General project answer | `03-resume-projects/01-project-answer-framework.md` |
| SLAM architecture | `03-resume-projects/02-slam-system-and-data-flow.md` |
| SLAM threads/rendering/memory | `03-resume-projects/03-slam-thread-render-memory.md` |
| AI platform loop | `03-resume-projects/04-ai-platform-business-loop.md` |
| AI reliability/cost | `03-resume-projects/05-ai-output-persistence-and-cost.md` |
| Project truth and metrics | `03-resume-projects/06-truth-boundaries-and-metrics.md` |
| Web/auth/backend | `04-backend-for-agent-and-payment/01-http-rest-auth-and-security.md` |
| Django | `04-backend-for-agent-and-payment/02-django-request-and-service-layers.md` |
| Database | `04-backend-for-agent-and-payment/03-data-model-transactions-and-indexes.md` |
| Redis/cache | `04-backend-for-agent-and-payment/04-redis-cache-and-consistency.md` |
| Async/retry/idempotency | `04-backend-for-agent-and-payment/05-async-jobs-retry-and-idempotency.md` |
| Reliability/observability | `04-backend-for-agent-and-payment/06-logging-tracing-deployment.md` |
| Order/payment/ledger concepts | `05-payment-engineering/01-order-payment-and-ledger-models.md` |
| Stripe Checkout/PaymentIntent | `05-payment-engineering/02-stripe-checkout-paymentintent-flow.md` |
| Webhook/signature/idempotency | `05-payment-engineering/03-webhook-signature-and-idempotency.md` |
| Payment state machine/transactions | `05-payment-engineering/04-payment-state-machine-and-transactions.md` |
| Refund/reconciliation/recovery | `05-payment-engineering/05-refund-reconciliation-and-recovery.md` |
| Payment interview drill | `05-payment-engineering/06-payment-interview-defense.md` |
| Agent/workflow/loop | `06-agent-engineering/01-agent-workflow-and-agent-loop.md` |
| Tool use/function calling | `06-agent-engineering/02-tool-use-and-function-calling.md` |
| MCP resources/tools/prompts | `06-agent-engineering/03-mcp-resources-tools-and-prompts.md` |
| RAG/context/memory | `06-agent-engineering/04-rag-context-and-memory.md` |
| Agent backend service | `06-agent-engineering/05-agent-backend-service-architecture.md` |
| Evals/tracing/guardrails | `06-agent-engineering/06-evals-tracing-and-guardrails.md` |
| Agent interview drill | `06-agent-engineering/07-agent-interview-defense.md` |

Repeated daily tasks may point to the same article; no task may point to two competing canonical articles for the same topic.

- [ ] **Step 3: Add task-level execution fields without changing the README table shape**

Use the full `daily-plan.md` columns: 日期、阶段、编号、任务、优先级、预计小时、MD 笔记、推荐教程/资料、完成产物、状态、面试后返工. Initialize status as `未开始` and返工 as `—`.

- [ ] **Step 4: Make the README resource cells actionable**

For each 7/18–7/24 row, reserve 2–4 direct must-use resource links plus `[当日完整资源](08-resources/02-july-18-to-24-must-use.md#date-anchor)`. Do not use the link label `教程` by itself.

- [ ] **Step 5: Verify schedule coverage**

Run checks that every task row has priority, canonical MD link, resource link or explicit `招聘平台/项目代码/错题本`, completion output, and status. Expected uncovered P0 tasks: `0`.

- [ ] **Step 6: Commit the schedule remap**

```powershell
git add README.md daily-plan.md 00-start-here/03-july-18-to-24-sprint.md
git commit -m "docs: remap sprint schedule to canonical notes"
```

---

### Task 4: Research and rebuild the resource system

**Files:**
- Modify: `08-resources/01-resource-selection-rules.md`
- Modify: `08-resources/02-july-18-to-24-must-use.md`
- Modify: `08-resources/03-android-learning-path.md`
- Modify: `08-resources/04-project-backend-payment-path.md`
- Modify: `08-resources/05-agent-learning-path.md`
- Modify: `08-resources/06-after-july-24-reference.md`
- Modify: `08-resources/README.md`
- Modify: `daily-plan.md`
- Modify: `README.md`

**Interfaces:**
- Consumes: Date/task IDs and canonical note paths from Task 3.
- Produces: Verified exact URLs for the README summary, daily plan, and topic paths.

- [ ] **Step 1: Build a P0 coverage ledger**

List every distinct 7/18–7/23 P0 task in `08-resources/02-july-18-to-24-must-use.md` under date anchors `2026-07-18` through `2026-07-23`. For each task record: task ID, note link, one or two must-use resources, suggested range, estimated minutes, explanation characteristic, answer produced, source class, and verification date `2026-07-18`.

- [ ] **Step 2: Verify current and replacement resources on the web**

Use current web search because availability, popularity, and documentation paths can change. Prefer official Android codelabs/courses, Kotlin/Java/Square/Stripe/OpenAI primary docs, and exact project examples. Add vivid or high-reputation Chinese/video tutorials when they outperform official references for speed; record why they were selected. Reject search-result pages, author profiles, generic homepages, unverifiable future-dated claims, and links that do not open.

- [ ] **Step 3: Populate the daily must-use page**

Keep one or two must-use links per task. Complex topics should normally pair a fast explanation with a primary reference, but a single exceptional resource is allowed when it is sufficiently complete. Put overflow links in `补充` or `7 月 24 日后`, never in the README cell.

- [ ] **Step 4: Populate the three topic learning paths**

`03-android-learning-path.md` covers Java/Kotlin minimums, Android platform fundamentals, modern stack, and the demo map. `04-project-backend-payment-path.md` covers SLAM, AI platform, backend foundation, and Stripe. `05-agent-learning-path.md` covers Agent loop, tools, MCP, RAG/context, backend service architecture, evals/tracing, and interview defense. Reuse the daily page links by reference; do not duplicate annotations verbatim.

- [ ] **Step 5: Move long references after the deadline**

Place comprehensive documentation, books, long playlists, advanced Framework/performance material, deep payment operations, and extended Agent evaluations in `06-after-july-24-reference.md`.

- [ ] **Step 6: Backfill exact resource links into the schedule and README**

Every 7/18–7/24 README row receives 2–4 direct links plus its complete daily anchor. Every P0 task row in `daily-plan.md` receives at least one exact resource link.

- [ ] **Step 7: Verify resource coverage and link quality**

Expected results: `UNCOVERED_P0_TASKS=0`, `GENERIC_TUTORIAL_LABELS=0`, `SEARCH_PHRASE_ENTRIES=0`, and every external link has a verification note or is a non-web personal input such as project code or错题本.

- [ ] **Step 8: Commit the resource rebuild**

```powershell
git add README.md daily-plan.md 08-resources
git commit -m "docs: rebuild verified sprint resources"
```

---

### Task 5: Remove superseded structure and prepare Feishu sync

**Files:**
- Delete: `00-goals-and-date/`
- Delete: `01-learning-order/`
- Delete: `02-android-basics/`
- Delete: `03-mvvm-jetpack-architecture/`
- Delete: `04-jetpack-compose/`
- Delete: `05-retrofit-okhttp-network/`
- Delete: `06-resume-project-defense/`
- Delete: `07-payment-engineering/`
- Delete: `08-agent-development/`
- Delete: `09-resources/`
- Delete: `10-recite-checklist/`
- Delete: `11-interview-strategy/`
- Delete: `12-java-basics/`
- Delete: `13-backend-basics/`
- Delete: `table-sync-placeholder.md`
- Create: `docs/feishu-sync/2026-07-18-update-checklist.md`
- Modify: `README.md`

**Interfaces:**
- Consumes: All stable navigation and resource paths from Tasks 1–4.
- Produces: A repository with no duplicate outline and a copy-ready Feishu update package.

- [ ] **Step 1: Confirm no unique article body would be lost**

Inspect every old article outside `09-resources`. Expected: only title, placeholder status, and outline markers. Preserve the resource decisions by completing Task 4 before deleting `09-resources`.

- [ ] **Step 2: Delete superseded directories and placeholder with `apply_patch`**

Delete only the exact paths listed in this task. Do not delete `docs/superpowers`, `.gitignore`, `LICENSE`, `README.md`, `daily-plan.md`, or `article-template.md`.

- [ ] **Step 3: Create the Feishu update checklist**

Include: the three Feishu source URLs; the GitHub canonical-path rule; the five-column daily table header; one copy-ready row per date; the resource-page links for each day; the new column map; obsolete GitHub paths to replace; and a checkbox noting that actual Feishu writeback is blocked until an authenticated edit connector is available.

- [ ] **Step 4: Scan for old path references**

Run:

```powershell
$old = '00-goals-and-date|01-learning-order|02-android-basics|03-mvvm-jetpack-architecture|04-jetpack-compose|05-retrofit-okhttp-network|06-resume-project-defense|07-payment-engineering|08-agent-development|09-resources|10-recite-checklist|11-interview-strategy|12-java-basics|13-backend-basics|table-sync-placeholder'
$hits = Get-ChildItem -Recurse -Filter *.md | Select-String -Pattern $old
"OLD_PATH_REFERENCES=$($hits.Count)"
```

Expected: `OLD_PATH_REFERENCES=0`, excluding historical design and plan documents under `docs/superpowers` when reporting migration evidence.

- [ ] **Step 5: Commit cleanup and sync package**

```powershell
git add -A
git commit -m "docs: remove duplicate outline and prepare Feishu sync"
```

---

### Task 6: Verify and publish the repository

**Files:**
- Inspect: all tracked Markdown files
- Modify only if verification finds a concrete defect.

**Interfaces:**
- Consumes: Completed repository from Tasks 1–5.
- Produces: Verified commits pushed to `origin/master`.

- [ ] **Step 1: Check Markdown formatting and repository state**

Run:

```powershell
git diff --check HEAD~5..HEAD
git status --short --branch
```

Expected: no whitespace errors and a clean worktree ahead of `origin/master`.

- [ ] **Step 2: Check every relative Markdown link**

Run:

```powershell
$broken = foreach ($file in Get-ChildItem -Recurse -Filter *.md) {
  $text = Get-Content $file.FullName -Raw -Encoding utf8
  foreach ($match in [regex]::Matches($text, '\[[^\]]+\]\(([^)]+)\)')) {
    $target = $match.Groups[1].Value
    if ($target -match '^(https?://|mailto:|#)') { continue }
    $pathOnly = [uri]::UnescapeDataString(($target -split '#')[0])
    $resolved = Join-Path $file.DirectoryName $pathOnly
    if (-not (Test-Path -LiteralPath $resolved)) { "$($file.FullName) -> $target" }
  }
}
"BROKEN_LOCAL_LINKS=$($broken.Count)"
```

Expected: `BROKEN_LOCAL_LINKS=0`.

- [ ] **Step 3: Check article and schedule invariants**

Expected: nine top-level columns; no old top-level numbered columns; every non-resource article linked from exactly one column README; no uncovered P0 task; README daily table has exactly five columns; each 7/18–7/24 row has 2–4 direct resources plus one daily anchor; shell articles still contain `状态：正文待写` and no technical body.

- [ ] **Step 4: Recheck external resource samples**

Open every must-use URL and a representative sample of supplemental links. Replace broken or redirected-to-login resources before publishing. Expected: every must-use link usable without relying on an inaccessible private session.

- [ ] **Step 5: Inspect final history and diff summary**

Run:

```powershell
git log --oneline --decorate -10
git diff --stat origin/master..HEAD
```

Expected: design and plan commits followed by five focused implementation commits; changes limited to Markdown structure, resources, and navigation.

- [ ] **Step 6: Push GitHub**

Use the GitHub publish workflow, then run:

```powershell
git push origin master
git status --short --branch
```

Expected: `master...origin/master` with a clean worktree.

- [ ] **Step 7: Report the Feishu boundary**

Provide the path to `docs/feishu-sync/2026-07-18-update-checklist.md`, state that GitHub is updated, and request an authenticated Feishu edit connector only for the remaining writeback.

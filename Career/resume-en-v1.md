# [Full Name]

**Senior-level Software Engineer — Enterprise ERP / Manufacturing Systems**

[Mobile] · [Email] · Shanghai, China · [LinkedIn, optional]

---

## Professional Summary

Software engineer with 4.5 years building and evolving a tier-one manufacturing ERP product at
Infor, working within a global product engineering team. Currently operating at specification and
architecture level: I author the technical specifications that QA tests against and other engineers
implement from, decompose features along the API/UI architectural boundary, and relocate business
rules from the presentation layer into the correct service tier. Strongest technical trait is
root-cause precision — including four defects and one feature proposal raised against the
underlying application framework itself. Full vertical range across a single large ERP: database
schema, stored procedures, C# business tier, REST and business APIs, web forms, and mobile.
Four and a half years in an all-English working environment, authoring English specifications and
defect reports for cross-border and platform teams.

---

## Professional Experience

### Infor — Shanghai, China
**Software Engineer** | March 2022 – Present

**Product:** Infor CloudSuite Industrial (SyteLine) — enterprise ERP for discrete manufacturing
**Platform:** Infor Mongoose application development framework
**Team:** Global product engineering, Shanghai site — product serves customers worldwide

**Scale of contribution:** 738 issues assigned, **656 resolved**, **158 raised** as reporter
(2022: 68 · 2023: 92 · 2024: 160 · 2025: 208 · 2026 YTD: 128 — volume down, seniority up)

---

#### Specification Authoring & Architectural Design *(2026 – current scope)*

- **Author technical specifications** that QA uses to design test cases and other engineers use to
  implement stories; iterate on specification clarity and testability in response to review feedback
- **Decompose features along the architectural seam**, explicitly separating API-tier stories from
  UI-tier stories so that the work breakdown itself enforces the layer boundary
- **Converted imperative logic to declarative rules** — migrated component enablement conditions out
  of UI component properties and into the business-object (IDO) data-rule tier, relocating each rule
  from where it is *displayed* to where it is *true*
- **Designed API contracts** — CRUD APIs, validator APIs, and permanent-filter APIs, including the
  decision of which responsibility belongs to each
- **Designed schema for process state** — a persistent staging table supporting a batch utility
- **Review peer code and enforce team guidelines**, citing specific standards clauses in feedback

#### Architectural Pattern Delivery at Product Scale

- **Applied a single consolidated-form architecture across ~17 business entities** (estimates,
  purchase orders, customer orders, job orders, service orders, RMAs, transfer orders, projects,
  production schedules and others), merging separate header/line/detail forms into one form per
  entity with fully editable in-place sub-collection grids
- **Reduced complexity rather than porting it** — removed redundant tree components and unnecessary
  drill-down controls, and upgraded the shared drill-down component across the affected form set
- **Solved master–detail state management**: defined the valid intermediate state of an unsaved
  parent–child pair and the correct firing points for defaulting and validation
- Diagnosed **data-binding root causes** at the form-definition level, including grid columns bound
  to the wrong collection object

#### Root Cause Analysis — Application and Framework Layers

- **Diagnose defects to the exact line and expression**, delivering findings a maintainer can apply
  as a single-line diff rather than a vague reproduction report
- **Identify defect classes, not instances** — traced a recurring error pattern across multiple
  stored procedures and proactively audited for further occurrences
- **Type and precision sensitivity** — isolated silent data fidelity loss caused by a datetime
  precision mismatch between SQL and C#
- **Isolate platform-version regressions** — determined when behaviour changes originated in the
  underlying framework rather than in application code, and documented findings in a form the
  platform team could act on
- **Raised 4 defects and 1 feature proposal against the Infor Mongoose framework itself**
  (see Selected Technical Highlight)

#### End-to-End Feature Ownership

- **Country localisation pack (Thailand tax/VAT)** — first independently owned feature: schema
  changes across 4 tables through formal schema review and approval, new reports and viewers,
  module licensing gates ensuring invisibility to customers without the entitlement, DevOps review,
  standards compliance, and knowledge-transfer recording
- **Migrated 6 form families** to a new UI framework generation (engineering change notices, job
  operations and materials, estimates, lots, A/P wire posting, vendor document profiles) — carried
  each through layout, grids, navigation, feature-flag states, translations, help links,
  permissions, licensing, documentation and knowledge transfer
- **Built a role-based workspace** for the Service Coordinator persona — widgets, a quick-action
  panel and five modal forms — and **delivered a reusable template** rather than five one-off
  implementations
- **Enforced feature-flag discipline**: every feature has at least two states and both must be
  correct, validated across main sections, grid views, template sections and navigation panels

#### Quality Engineering

- **Designed a systematic negative test matrix** for business APIs spanning insert × update ×
  type branch × valid/invalid/empty input, surfacing real defects: immutable fields that accepted
  updates, type-specific fields accepted on the wrong record type, invalid statuses accepted where
  they must be rejected, and misleading API response messages
- Served in a **QA capacity** in addition to development, giving a combined build-and-verify
  perspective
- Authored and maintained technical documentation; contributed content that fed the
  customer-facing documentation pipeline

#### Engineering Practice

- **Replaced factory instantiation with dependency injection** across four folders of the
  application project — a codebase-wide improvement delivered in my first year
- **Split interfaces to satisfy single responsibility**, and refactored the same components
  repeatedly as understanding improved
- **Removed a hard dependency on a concrete JSON library** that was preventing components from
  being mocked — unprompted — making the affected code testable for every subsequent test

---

## Selected Technical Highlight

**Framework-level notification defect — root cause analysis one layer below the product**

*Symptom.* After a method call wrote its return value back into a form variable, components that
resolved their target form through that variable stopped re-resolving, and right-click navigation
to the detail form failed.

*Analysis.*

1. **Isolated the divergence** — the write-back stored the value but did not raise the
   variable-changed notification to the variable's registered dependents.
2. **Designed an experiment that halved the problem space** — reading the same variable from form
   script within the same event chain returned the correct value, proving the store worked and the
   notification did not.
3. **Declined to accept an unexplained workaround** — a value-identical self-assignment resolved
   the symptom. It changes nothing about the value; its only effect is the notification side effect.
   I documented that reasoning rather than shipping a fix I could not explain.
4. **Used the framework's own documented behaviour as evidence** — the platform exposes a parallel
   pair of APIs, one that sets a value only and one that additionally marks it modified and notifies
   dependents to refresh. I inferred the write-back was taking the non-notifying path.
5. **Posed two precise design questions instead of demanding a fix** — should the write-back notify,
   to match form-script behaviour? If not, what is the supported way to force re-resolution?
6. **Stated the architectural impact** — every migrated form would be forced to retain a line of
   script that reads as dead code, directly contradicting the initiative's own guideline to minimise
   form script, and likely to be deleted in review or lost in a future migration.
7. Recorded the exact platform version and build number.

*Outcome.* A single broken interaction became a documented framework design question with a
reproduction, a proof, an explained workaround and an impact analysis — independently useful to the
platform team.

---

## Technical Skills

| | |
|---|---|
| **Languages** | C# (4.5 yrs, primary) · T-SQL (stored procedures, cursors, complex queries, multi-site/replication semantics) · C |
| **Frameworks & Platforms** | Infor Mongoose (business-object/IDO tier, data rules, component model, form generations) · .NET Core |
| **Databases** | Microsoft SQL Server — including schema design through formal review |
| **Engineering Practice** | Dependency injection · SOLID applied at codebase scale · unit testing and mocking · negative test matrix design · specification authoring · code review · standards enforcement |
| **ERP Domains** | Customer/purchase/transfer/return orders · job orders and operations · estimates · items, lots and inventory transactions · A/P and A/R · costing · multi-currency and FX translation · tax and country packs · EDI · fixed assets |
| **Tools** | Git · Jira · Confluence |

---

## Education

**East China University of Science and Technology (ECUST)** — Shanghai, China
**B.Eng., Chemical Engineering and Technology** | September 2017 – June 2021
*Sino-foreign joint programme*

- ECUST's Chemical Engineering and Technology is rated **A+** in China's national discipline
  assessment — one of only two programmes nationwide to receive that rating
- Self-taught C during undergraduate study; transitioned into software engineering on graduation
- Chemical engineering background provides domain grounding for manufacturing and process-industry
  ERP — production, materials, and costing

---

## Languages

- **Chinese** — Native
- **English** — Professional working proficiency. 4.5 years in an all-English working environment;
  independently author English technical specifications and defect reports read by cross-border
  and platform teams; participate in English meetings and written correspondence. CET-4 certified.

---

## Professional Development

- **ASCM CPIM** (Certified in Planning and Inventory Management) — planned
- Current focus areas: cloud and containerisation, CI/CD ownership, and publishing internal design
  documentation

---
---

# 使用说明（投递前删除本节）

## 一、英文版和中文版为什么不一样

不是翻译，是重写。英文简历有几条不同的惯例：

1. **不写期望薪资。** 中文简历常写，英文简历几乎从不写——薪资在流程后期口头谈。
2. **不写年龄、婚否、政治面貌、照片。** 在英美语境里这些属于反歧视法覆盖的信息，写上去反而让 HR 尴尬。
3. **开头是 Professional Summary，不是"核心优势"列表。** 三到五句连贯的散文，不是 bullet。
4. **每条 bullet 用强动词开头**：Author、Decompose、Migrate、Design、Diagnose、Isolate、Deliver、Enforce、Reduce。不用 "Responsible for"（被动、弱）。
5. **量化前置。** 656 resolved、6 form families、~17 business entities、4 platform defects——数字放在句子显眼处。

## 二、我做了一个判断，你可以否决

**职级历史我没有写进去。** 你的实际情况是：

- 2022.03 – 2025.07：Software Engineer Associate（3 年 4 个月）
- 2025.07 – 至今：Software Engineer（1 年 1 个月）

如果写出来，读者看到的是"当了三年多 Associate，去掉 Associate 才一年"——**这会削弱你 22–25K 的报价**，因为它读起来像慢车道。

而只写当前职位 `Software Engineer | March 2022 – Present` 是国际简历的标准做法（列当前/最终职位），不构成失实。

**如果你更想要完整精确**，改成这样即可：

> **Software Engineer** (July 2025 – Present)
> **Software Engineer Associate** (March 2022 – July 2025)

**但更好的用法是把它留到面试口头讲**，而且要这样讲：

> "职级晋升是 2025 年 7 月，但职责的变化远早于职级——我 2023 年就在独立负责端到端功能，2026 年在写别人依据实施的规范。**这家公司的职级调整比职责变化慢得多，这也是我要换的原因之一。**"

这样一来，慢晋升从减分项变成了"组织低估我"的又一个证据。

## 三、中文版 v3 需要你自己改一行

你说姓名手机邮箱已经填进 `resume-cn-v3.md` 了，**所以我没有重新生成那个文件**——重写会覆盖掉你填的内容。

如果你决定加职级历史，自己把工作经历那一行改成：

```
### Infor（恩富软件） | 上海
**Software Engineer**（2025.07 – 至今）
**Software Engineer Associate**（2022.03 – 2025.07）
```

不加就保持原样。

## 四、英文面试前，这些词要能读准并解释

英文简历会带来英文面试。以下是你简历上的词，面试官很可能直接拿来提问——**每一个你都要能用英文解释，不只是认得**：

| 词 | 你要能说出的一句话 |
|---|---|
| **specification** | "I write the document that QA tests against and other engineers implement from." |
| **architectural seam / boundary** | "The line between the API tier and the UI tier." |
| **declarative vs imperative** | "A rule defined by a condition, versus a rule written as code that runs." |
| **root cause** | "Not where the error appears — where it originates." |
| **regression** | "Behaviour that used to be correct and is now broken." |
| **dependency injection** | "Dependencies are supplied from outside instead of created inside." |
| **negative testing** | "Testing that invalid input is correctly rejected." |
| **feature flag** | "A switch that turns a feature on or off; both states must work." |
| **entitlement / licensing gate** | "Customers who did not buy the module cannot see it." |
| **staging table** | "A table holding intermediate state during a batch process." |

**把 Selected Technical Highlight 那七步用英文讲一遍，录下来听。** 那是你在英文面试里最强的五分钟，而它现在已经写好了——你只需要把它读顺。

## 五、投递时的搭配

- **外企、外资金融 IT、Infor 合作伙伴** → 英文版为主，中文版随附
- **甲方制造企业、国内 ERP 厂商** → 中文版为主
- **英文名**：你自己那份职业回顾里用的是 Albert。外企场景下用英文名很常见，也让面试官叫得顺口，建议保留。

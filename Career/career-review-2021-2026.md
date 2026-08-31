# Career Review — Albert Zhang (张一昌)

**Purpose of this file.** So I stop muddling along, unsure of what I am doing and what I
have already done. Every claim below is backed by a real Jira issue key I can open.

- **Graduated (bachelor's):** June 2021
- **Started working:** March 2022 — Infor, CloudSuite Industrial (SyteLine), Software Engineer
- **This review written:** 2026-08-31 (4 years 6 months of work; 5 years 3 months since graduation)
- **Evidence source:** Atlassian (infor.atlassian.net) — Jira + Confluence, pulled 2026-08-31

---

## 0. The numbers

| Metric                            | Value                                         |
| --------------------------------- | --------------------------------------------- |
| Jira issues ever assigned to me   | **738**                                 |
| Issues resolved                   | **656**                                 |
| Issues I raised myself (reporter) | **158**                                 |
| Projects worked in                | CSIB (725), MGD, TECDOC, JIRA                 |
| Confluence pages I created        | **1** (my own profile page, 2023-02-28) |

Resolved per year:

| Year     | Resolved | Note                                                        |
| -------- | -------- | ----------------------------------------------------------- |
| 2022     | 68       | First 10 months. Learning the codebase.                     |
| 2023     | 92       | First owned feature (Thai Country Pack).                    |
| 2024     | 160      | Owning Gen2 forms end-to-end.                               |
| 2025     | 208      | Peak volume. IDS migration at scale.                        |
| 2026 YTD | 128      | Volume down,**level up** — architecture + spec work. |

**Read the last two rows carefully.** 2025 was my highest count. 2026 is lower but is by far
my most senior work. Ticket count is not seniority. Do not chase the count again.

### My starting point (for honest comparison)

March 2022, what I actually had:

- Basic computer science fundamentals
- Basic C
- Basic C# syntax
- A rough, textbook-level understanding of the SOLID principles — could name them, had never applied them

---

## 1. Project: C#izer — Stored Procedure → C# Conversion

**Period:** 2022 – mid 2023 (bulk of it), tickets created 2021-03 before I joined
**Scale:** Dozens of `C#izer - Conversion - *Sp` tickets, plus a second wave of `Group *Sp` tickets
**Representative issues:** CSIB-38396 (APQPCustUpdSp), CSIB-38734 (AU_RepriceCoitemorBlanketLinesSp),
CSIB-39280 (CLM_ApsGetORDERSp), CSIB-41398 (InvoiceTableUpdSp), CSIB-41453 (Item_ItemRevSp),
CSIB-42495/42496 (ProcplnDelSp / ProcplnInsSp), CSIB-43706 (SSSFSConsoleTransSaveSp),
CSIB-44604 (ValidateLocationForExternalWarehouseSp), CSIB-51182 / 51272 / 51498 (SQL functions),
CSIB-67373 / 67382 (Group ecniJobSp / Group PmatlValidateMatlQtySp)

### What it actually was

Translating legacy T-SQL stored procedures into C# so the business logic could live in the
application tier instead of the database. Labels on my tickets show the taxonomy I worked
through: `StoredProcedure`, `Function`, `Validator`, `BothInSQLAndC#`, `QASHTPReview`.

This was my onboarding assignment. The tickets were created in bulk in March 2021 — before I
existed at the company — and handed to me. Fully specified work, no design freedom.

### Key skills I learned

- **Reading T-SQL fluently** — cursors, temp tables, `@Infobar` output parameters, multi-plant
  and multi-site logic, replication concerns
- **Behaviour-preserving translation** — the discipline that the C# must produce *identical*
  results to the SQL, not "reasonable" results
- **The SyteLine/Mongoose IDO layer** — how business logic is invoked, what an IDO method
  signature means, how SPs and C# coexist during a migration
- **Real domain knowledge**: orders, jobs, estimates, inventory, A/P, A/R, costing. This is the
  asset I underrate. It is why I can now tell a UI bug from a business-rule bug in seconds.

### Hardest problem I struggled with

**CSIB-67244 — "MsgAppSp: The results are not consistent between SQL and C#."**

The conversion compiled, the tests passed, and the two implementations still disagreed. This
is the hardest class of bug there is: no crash, no error, just two answers. I had to stop
trusting "it looks equivalent" and start proving equivalence case by case. The `BothInSQLAndC#`
label on many of my tickets exists precisely because both versions run in parallel and must
agree.

The same lesson repeats in CSIB-77630 — `ApsBOMSaveSp will result in a loss of datetime precision`. Not a logic error. A **type fidelity** error. SQL `datetime` and the C# type I used
did not round-trip. Silent data corruption.

### My biggest contribution

Volume with correctness, in a domain I did not know, on code nobody wanted to touch. Unglamorous
and genuinely valuable. But the real contribution was to myself: this project is where I stopped
being a graduate. By the end I could read any SP in the product and say what it did.

### Verdict

Necessary. Not something to be proud of forever. **I should not still be doing work like this.**

---

## 2. Project: IDO REST Layer — MessageParser / MessageProducer / ServicePathProvider

**Period:** Feb 2022 – Nov 2022
**Representative issues:** CSIB-57194 (UT: GetServiceUrl), CSIB-58247 (CUT: ServicePathProvider),
CSIB-58261 (CUT: MessageProducer), CSIB-58275 (CUT: MessageParser), CSIB-58289 (CUT: Invoke REST
from IDO method), CSIB-58613 / 58617 / 59655 (unit tests), CSIB-59382, CSIB-59898, CSIB-59970,
CSIB-60000, CSIB-60001, CSIB-60040, CSIB-60900, CSIB-61495, CSIB-61710, CSIB-61914, CSIB-61979
**Cross-cutting refactor:** CSIB-57981 (Adapters), CSIB-57994 (MXLOC), CSIB-57995 (NonTrans),
CSIB-58001 (Test) — *"Applying DI to get an instance instead of Factory on IDO method definition"*

### What it actually was

Building the capability to **invoke a REST service from inside an IDO method**: produce the
request message, perform the request, parse the response into DataTables and output parameters.
Then hardening it through several rounds of refactoring.

**This is the single most formative project of my career so far.** It is where the textbook
became muscle memory.

### Key skills I learned

- **Dependency Injection replacing Factory** — CSIB-57981/57994/57995/58001, applied folder by
  folder across the whole App project. This is the **D** in SOLID, done to a real production
  codebase, not an exercise.
- **Interface Segregation / Single Responsibility** — CSIB-59898, literally titled
  *"Refactor: split interfaces to meet single responsibility principle."* Then CSIB-60040
  *"Refactor MessageProducer"* and CSIB-59970 *"Refactor MessageProducer and MessageParser"* —
  I refactored the same components repeatedly as I understood them better. That is normal and
  healthy.
- **Testability as a design property, not a phase** — CSIB-59382: *"fix the use of
  newtonsoft.json in MessageParser. And mock the parse method in UT."* I noticed a hard
  dependency on a concrete JSON library was preventing me from mocking, and I removed it.
  Nobody told me to. **That is the exact moment SOLID stopped being trivia.**
- **Factory pattern used deliberately** — CSIB-60001: using `MessageParserFactory` to create the
  right parser for the response. I learned when a factory is the *right* answer, not just that
  DI is fashionable.
- **Unit testing and mocking** — `UT:` and `CUT:` tickets throughout. My first real test suites.
- **Not reinventing utilities** — CSIB-61914: *"Use the DateTimeUtil instead of the DateTime
  class."* Respecting a codebase's existing abstractions.

### Hardest problem I struggled with

**CSIB-61710 — "The nodes in the response json cannot be resolved"**, followed by **CSIB-61979 —
"Refine JSON's templates, optimize the parsing process for DataTable and OutputParameters."**

Parsing an arbitrary JSON response into two structurally different targets — a tabular DataTable
and a flat set of output parameters — through a template. My first genuine *design* problem: not
"make this work" but "what is the right shape for this?" I had to think about the abstraction
before writing code, and I got it wrong at least twice (hence the repeated refactor tickets).

Honourable mention: **CSIB-61495 — "Spell mistakes and Variable content mistakes caused debug
error in other issue."** My typos broke someone else's debugging session. A cheap and permanent
lesson in blast radius.

### My biggest contribution

Two things:

1. **The DI sweep (CSIB-57981/57994/57995/58001).** I did not just build my feature; I changed
   how instances are obtained across four folders of the App project. That is a codebase-wide
   improvement, and it was early in my career.
2. **Making the REST-from-IDO capability testable.** By removing the concrete Newtonsoft
   dependency and splitting the interfaces, I turned a hard-to-test component into a mockable
   one. Every later test on that code was cheaper because of it.

### Verdict

**This is the project I should talk about in any interview or promotion discussion.** It shows
principle applied under real constraints, plus the self-awareness to refactor my own design
repeatedly. It also proves the SOLID knowledge I claimed in 2022 became real in 2022.

---

## 3. Project: Enable Replication Triggers (Multi-Site Infrastructure)

**Period:** Sep – Oct 2022
**Representative issues:** CSIB-64536 (ChartAcctRemoteSp), CSIB-64542 (DelCoBlnSp),
CSIB-64543 (DeleteCoitemSp), CSIB-64544 (DeleteCoSp), CSIB-64545 (EuroCustSp),
CSIB-64547 (JobCopySp), CSIB-64549 (JobtPcISp), CSIB-64555 (psitem_mstDel),
CSIB-64560 (rmaitem_mstIup), CSIB-64561 (Rpt_JobMaterialPickListSp),
CSIB-64566 (UpdateOldInvoiceNumSp), CSIB-64569/64570/64571/64572 (SSSFS* procedures)

### What it actually was

A systematic sweep, roughly 15+ tickets in one month, enabling replication triggers so that
data changes propagate correctly across sites in a multi-site SyteLine deployment.

### Key skills I learned

- **Multi-site / replication semantics** — why a delete in one site must be visible in another,
  and what breaks when a trigger is missing
- **Working at sweep scale** — batching near-identical changes without losing accuracy on any
  single one; recognising which of the 15 is *not* actually identical
- The habit of treating a large uniform task as a checklist, not 15 unrelated tasks

### Hardest problem I struggled with

Nothing intellectually hard here. The real difficulty was **sustaining attention on repetitive
work**, where the cost of one careless ticket is a data-consistency bug in production that
nobody will trace back to me for months.

### My biggest contribution

Reliability at volume. This is the kind of task a team gives to someone it trusts not to skip a
step.

### Verdict

Low-growth, high-trust work. Fine at the time. **Should not recur.**

---

## 4. Project: Thai Country Pack (First Feature I Owned)

**Period:** late 2022 – 2023
**Representative issues:** CSIB-63063 (parent feature), CSIB-67243 (Thai Input VAT Report),
CSIB-67117 (THAInputVatReport column alignment), CSIB-68431 (create THASalesVATRegisterReport +
Viewer), CSIB-68416 / 68566 / 68615 (add Head Office & Branch Name to Tax Parameters, Customers,
Multi-Site Customers), CSIB-68567 (schema changes: `customer_mst`, `taxparms_mst`,
`customer_mst_all`, `taxparms_mst_all`), CSIB-69902 (Country Pack module control on Thai forms),
CSIB-68422 (DevOps Review), CSIB-68424 (Standards and Guidelines), CSIB-68442 (Knowledge Transfer
Recording), CSIB-71492 / 71526 (Schema Review/Approval)

### What it actually was

Thailand-specific tax and VAT functionality: new report forms, new fields on existing forms,
the database schema behind them, and the module/licence gating that keeps a country pack from
leaking into other customers' installations.

**This is the transition point in my whole career.** Before it: I converted other people's
procedures. From here on: I add fields, change schemas, create forms, and get reviewed on it.

### Key skills I learned

- **Database schema design and review** — CSIB-68567 changed four tables, including `_all`
  variants. CSIB-71492 / 71526 are `Schema Review/Approval` tickets: my schema changes went
  through formal review. Learning that a schema change is a **contract**, not an edit.
- **Report development** — new forms plus their viewer counterparts
- **Feature gating** — CSIB-69902: `Add Country Pack Module control on Thai Related Forms`.
  Understanding that a feature must be *invisible* to customers who did not buy it.
- **Multi-site data modelling** — the `_mst` / `_mst_all` distinction
- **The full delivery lifecycle** — for the first time my work included DevOps Review
  (CSIB-68422), Standards and Guidelines (CSIB-68424), and Knowledge Transfer Recording
  (CSIB-68442). Code is a fraction of shipping.
- **Localisation thinking** — tax rules differ per country; the architecture must absorb that
  without forking

### Hardest problem I struggled with

Getting a **schema change approved**. Code can be rewritten; a shipped schema cannot. Learning
to justify every column — nullability, width, `_all` variant, upgrade path — to reviewers who
were right to push back. Slower and more uncomfortable than writing the code.

### My biggest contribution

I delivered a complete, gated, reviewed, documented country-specific feature — schema through
report — in my second year. And I did the unglamorous surrounding work (module control, standards,
knowledge transfer) rather than only the fun part.

### Verdict

**My first real end-to-end ownership.** This is the project that proves I can be given a
requirement rather than a task.

---

## 5. Project: SQL / Stored-Procedure Root-Cause Fixes (a continuous thread)

**Period:** 2023 – 2024, ongoing background work
**Representative issues:**

- CSIB-69945 — *"The second variable should be `@PEndInv` at line 137 in CheckPrefixSp"*
- CSIB-70132 — *"The code should be `SUBSTRING(@CoOrderSource,1,3)='ISS'` in ValidateSourceCoNumForCopySp line 210"*
- CSIB-70341 — same defect class in `ValidateTargetCoNumForCopySp` line 282
- CSIB-73983 — *"`lot.revision` column is missed in cursor TfiqCrs select statement for PhyinvLoadSp"*
- CSIB-75001 — *"Remove `AND itemrev.Plant = @sPlant` from the join on the itemrev table in Item_ItemRevSp"*
- CSIB-77630 — *"ApsBOMSaveSp will result in a loss of datetime precision"*
- CSIB-78179 — *"Parameter `@Infobar` is missed in ALTGEN and EXTGEN method for VatProceduralMarkingDefaultsUpdSp"*
- CSIB-75443 — *"Return `Invalid object name 'tmp_journal'` when call Rpt_JournalCompressSp"*
- CSIB-86211 — SP errors surfaced by running APITestTool in "Using Sp" mode

### What it actually was

Not a project — a **capability** I developed and kept exercising. Diagnosing defects down to the
exact line and exact expression in stored procedures across the whole product.

### Key skills I learned

- **Precision in bug reporting.** Look at those titles. Not "the form is broken" but "line 137,
  wrong variable, should be `@PEndInv`." A fix is a one-line diff for whoever picks it up.
- **Reading someone else's SQL under pressure** — cursors, joins, plant filters, temp tables
- **Spotting the *class* of a bug.** CSIB-70132 and CSIB-70341 are the same mistake in two
  procedures. I found the second one because I understood the first. That is the difference
  between fixing a bug and understanding a bug.
- **Type and precision awareness** — CSIB-77630, datetime precision loss
- **Tool-driven discovery** — CSIB-86211: using APITestTool's "Using Sp" mode to surface a class
  of defect systematically rather than waiting for reports

### Hardest problem I struggled with

CSIB-75001 — removing `AND itemrev.Plant = @sPlant` from a join. The hard part was not seeing
the line. It was being **confident enough to say a filter that has been in production for years
is wrong**, and reasoning through what it would break in multi-plant scenarios. Deleting a
condition takes more courage than adding one.

### My biggest contribution

I became the person who can say *where* the bug is, not just *that* there is one. This capability
is what later let me file framework-level defects against the Mongoose platform (see §10).

### Verdict

**This is my strongest and most transferable technical trait.** Everything senior I have done
since is built on it.

---

## 6. Project: Gen2 Form Family (ECN, Job Orders, Estimates, Lots, A/P, Vendor)

**Period:** 2023 – 2024
**Forms I owned:**

- **Engineering Change Notices / ECN Items / ECN Lines** — CSIB-80312 (CUT: New ECN Lines Form),
  plus ~15 defects: CSIB-85195, 85198, 85201, 85214, 85308, 85331, 85332, 85545, 86880, 86901,
  86911, 86947, 87351, 87560, 88409
- **Job Operations / Job Materials** — CSIB-80578, CSIB-80579, CSIB-85551, CSIB-85569, CSIB-85803,
  CSIB-85818, CSIB-86788, CSIB-86841, CSIB-86933, CSIB-87350
- **Estimates / Estimate Job Orders / Estimate Job Operations & Materials** — CSIB-78821,
  CSIB-95861, CSIB-95862, CSIB-97051, 97052, 97057, 97058, 97073, 97080, 97081, 97132, 97134,
  97138, CSIB-98752
- **Lots** — CSIB-85009 (CUT: Lots), CSIB-92938, CSIB-93914 (licence request)
- **A/P Wire Posting** — CSIB-87942 (CUT), CSIB-93425, CSIB-93755, CSIB-93756, CSIB-95047,
  CSIB-93919 (licence request)
- **Vendor Document Profile** — CSIB-87923 (CUT), plus ~13 defects: CSIB-94407 – 94415,
  CSIB-94465, 94466, 94515, 95014, 95015, 95016, CSIB-95321, CSIB-95500, CSIB-93917 (licence)
- **A/P Payment Distribution** — CSIB-92198
- **Supporting:** CSIB-88604 / 99898 / 99914 / 99930 / 99946 (Acceptance Tests),
  CSIB-88608 / 99870 (QA Test Writing), CSIB-84569 / 84588 / 84622 (Documentation),
  CSIB-91485 / 91900 / 92307 / 99912 / 99960 (Knowledge Transfer Recording)

### What it actually was

Migrating classic SyteLine forms to the Gen2 UI framework — and then owning every consequence:
layout, grids, sub-collections, right-click navigation, tooltips, required-field indicators,
duplicate-row numbering, feature flags, translations, help links, permissions, licences, docs.

### Key skills I learned

- **Front-end / UI framework work** — a genuinely new axis for me. Grids, sub-collection grids,
  navigational panels, modal forms, layout and scrollbar behaviour, tooltips, images
- **Feature-flag discipline** — CSIB-85569 (`Can not open Job Operations.gen2 when feature CSIB_73813 is on`), CSIB-92938 (error when the feature is *disabled*), CSIB-94409 / 94515 /
  95015 / 95016 (behaviour conditional on `CSIB_73389`). **Every feature has at least two states
  and both must work.** I learned this the hard way, repeatedly.
- **Behavioural parity as the acceptance criterion** — the new form must match the classic form,
  not merely function. Many tickets are literally "different from classic form."
- **Non-code delivery obligations** — licences (CSIB-93914/93917/93919), permissions,
  help links (CSIB-87350/87351), translations (CSIB-93906), documentation, feature descriptions
  (CSIB-95047, CSIB-94407)
- **Accessibility and usability judgement** — field sizes, ordering (CSIB-88409: "Manufacturer
  should be before Manufacturer Item"), disabled-state visual cues (CSIB-85818: "disabled but
  looks not in grey")
- **Absorbing a high volume of small defects without losing the thread**

### Hardest problem I struggled with

**The feature-flag matrix.** CSIB-85569 and CSIB-92938 are mirror images: one breaks with the
flag ON, one breaks with it OFF. On Vendor Document Profile I had to get the form right in both
states across the main section, the grid view, the email-template section, and the navigation
panel — CSIB-94409, 94515, 95015, 95016 are all the same underlying discipline. Combinatorial,
tedious, and easy to get 90% right, which is 0% right.

Runner-up: **CSIB-93906, "Gen2 forms not working correctly with Translations."** A whole class of
correctness I had not been thinking about at all.

### My biggest contribution

I converted **six form families** to Gen2 and carried each one all the way to shipping —
including the parts nobody thanks you for: licence requests, help IDs, permission groups,
translations, documentation, knowledge transfer. Delivery, not just development.

### Verdict

This is where I became a **full-stack** engineer on this product: schema → SP → C# → IDO → UI.
The work itself is not deep, but the breadth it bought me is real.

---

## 7. Project: Service Coordinator Workspace & QuickActions

**Period:** 2024 – 2025
**Representative issues:** CSIB-114536 (CUT: Story Req-6A — Quick Action Widget UI),
CSIB-114540 (Documentation: QuickActions_ServiceCoordinator.home), CSIB-114428
(ScheduledAppointmentsModal), CSIB-114572 (AddNotesModal), CSIB-114650 (ReviewWarrantiesModal),
CSIB-114714 (FinalizeInspectionsModal), CSIB-114590 (LookupKnowledgebaseArticlesModal),
CSIB-117029 (License Request for QuickActions), CSIB-119256 (Update QuickAction Template),
CSIB-120241 (Snooze list forms permission & licence checklist), CSIB-120292 (resolve form and
pop-up deficiencies), CSIB-120585 (Manifest file missing), CSIB-120833 (adjust initial size and
close button of pop-up modal), CSIB-119671 (widget form issues), CSIB-117722 (Vendor Hub KPI
total amount wrong), CSIB-119357 (L3-Apr25: error on launch-out icons on Vendor Hub.gen2)
**Docs shipped externally:** TECDOC-20824, TECDOC-22091

### What it actually was

Building a **role-based workspace** — a home screen for the Service Coordinator persona, made of
widgets, a QuickActions panel, and a family of modal forms (appointments, notes, warranties,
inspections, knowledge-base lookup). Plus the Vendor Hub KPI widgets.

Note the ticket vocabulary shift: `CUT: Story: Req-6A`. I am now working against **numbered
requirements**, in a proper QA cycle (`QA Test Writing` → `QA Test Execution` →
`Acceptance Tests` → `Documentation` → `Knowledge Transfer Recording`).

### Key skills I learned

- **Composite / persona-driven UI** — a workspace is not a form. Widgets, tiles, KPIs, snooze
  lists, and modals composed into one coherent screen for one job role
- **Templates and reuse** — CSIB-119256 `Update QuickAction Template`: building the pattern
  others instantiate, not just one instance
- **Modal form UX** — sizing, close buttons, pop-up behaviour (CSIB-120833, CSIB-120292)
- **Deployment artefacts** — CSIB-120585 `Manifest file missing`. A feature can be perfect and
  still not ship.
- **Permission & licence matrices at family scale** — CSIB-120241 is a whole checklist ticket
- **KPI / aggregate correctness** — CSIB-117722: a KPI showing the wrong total is worse than a
  KPI showing nothing, because people trust it
- **Writing for the doc team** — my features generated TECDOC tickets that became customer-facing
  documentation

### Hardest problem I struggled with

**CSIB-117722 — "Vendor hub cannot display the KPI total amount value correctly."** Aggregation
bugs are hard because there is no error; there is a plausible wrong number. I had to work back
from a displayed figure through the widget, the query, and the underlying business definition of
"total amount" — including currency and status filters — to find where the definition and the
implementation diverged.

The 2024 revenue-calculation tickets are the same species and are worth remembering together:
CSIB-101456 (*"the revenue calculation for the CO should also take into account the discount"*),
CSIB-101447 (*"shipping revenue for transfer order is wrong after full TO ship"*), CSIB-101491
(*"posted Material Shipment of Service Order in other currency should be converted to domestic
currency"*), CSIB-99901 (read total revenue of inventory in the widget). **Money maths is where I
learned that a "small" numeric bug is never small.**

### My biggest contribution

I delivered a complete persona workspace — widgets, QuickActions, five modal forms, permissions,
licences, manifest, documentation — and built a reusable QuickAction **template** rather than
five one-offs. That is a step from "I build features" toward "I build the thing features are
built from."

### Verdict

First project where I was clearly working at the **product design** level, not the ticket level.

---

## 8. Project: IDS Migration at Scale (Gen3)

**Period:** 2025 (my highest-volume year: 208 resolved)
**Batch conversion tickets (note the counts in the titles):**

- CSIB-124163 — `CUT: New Delete-Relative Utility IDS Form` **(18 forms)**
- CSIB-125009 — `CUT: New Finance-Relative Utility IDS Forms` **(11 forms)**
- CSIB-123289 — `CUT: New Reports related 5 IDS Form`
- CSIB-122425 — `CUT: AP AR Related IDS Forms`
- CSIB-123287 — `CUT: FixedAsset Reports`
- CSIB-123390 — `CUT: AddRmaReturnLine.ids AddShippingLine.ids`
- CSIB-123392 — `CUT: CTPResults IDS Forms`
- CSIB-121456 — `CUT: MobileParameters.ids`
- CSIB-122074 — `CUT: PP_PrintingIndustryParameters.ids`
- CSIB-127766 — `Gen3 IDS UX - IDS form CurrentOperations.ids for CurrentBOM.gen2`

**Domains covered:** EDI (CSIB-131952, 131954, 131958, 132145, 132149, 134800, 134801, 135012,
138949, 146187), Credit Card (CSIB-129802, 133357, 150553, 155036), Currency Codes (CSIB-132109,
150641, 150642), A/R reporting (CSIB-123751, 145856, 146023, 146279), printing industry
(CSIB-122335, 122874, 122875), CTP (CSIB-147296, 147302), Vendors (CSIB-146188, 146190),
mobile `*_mobi.ids` (CSIB-153578, 153692, 153829, 154090)
**Framework-version regressions:** CSIB-138588, CSIB-138611, CSIB-138949 — all
*"on Mongoose 2025.09.01"*
**Cross-cutting fixes:** CSIB-134041 (replace calculator icon with `icon-translate` across all
IDS forms), CSIB-134798 (update help IDs across a workspace)

### What it actually was

The next UI generation — converting the product's forms to IDS. Not one feature: **an industrial
programme**, dozens of forms per ticket, across most functional areas of an ERP.

### Key skills I learned

- **Working at programme scale.** "18 forms" in one ticket title changes how you work. You need
  a repeatable procedure, a self-check list, and a way to spot the odd one out.
- **Isolating framework-version regressions.** CSIB-138588 / 138611 / 138949 all say
  *"on Mongoose 2025.09.01"*. I learned to ask "did *my* code change, or did the *platform*
  change underneath me?" — a question junior engineers do not think to ask.
- **Cross-cutting consistency fixes** — CSIB-134041 and CSIB-134798 are single tickets that touch
  every form. Fixing a class, not an instance.
- **Mobile as a distinct target** — `*_mobi.ids`, different navigation and layout constraints
- **Genuine ERP breadth** — EDI, credit cards, currency, fixed assets, A/P, A/R, CTP, printing
  industry, projects. Few people on the team have touched this many areas.
- **Judging "is this the same as the classic form?" fast**, hundreds of times

### Hardest problem I struggled with

The framework-version regressions. When the same form is correct on one Mongoose build and wrong
on `2025.09.01`, the bug is not in front of you. Field order changes (CSIB-138588), a grid stops
adding a scrollbar (CSIB-138611), buttons that should be disabled are enabled (CSIB-138949). I had
to learn to **compare across platform versions**, not just against expected behaviour — and to
write the finding up in a way the platform team would accept.

Second: the sheer **sustained attention** of 208 issues in a year without quality drift.

### My biggest contribution

Volume and breadth that materially moved the IDS programme, plus the two cross-cutting fixes
(CSIB-134041, CSIB-134798) where I chose to fix the pattern everywhere instead of the one form in
front of me.

### Verdict

Impressive throughput; **shallow per ticket**. This is the year that taught me count ≠ level.
Its real value was that touching everything gave me a map of the whole product — which is exactly
what made the 2026 architecture work possible.

---

## 9. Project: Consolidated IDS Forms

**Period:** late 2025 – early 2026
**Programme tickets:** CSIB-155648 (Update Consolidated Form Layouts), CSIB-158892 / 159501 /
159504 / 159509 (*"Add and Maintain data directly in the SubCollection Grid"* for Customer Orders,
Purchase Orders, Estimates, PO Requisitions), CSIB-161147 (Uplift Drilldown control component)
**Per-entity layout work (one ticket each, I owned the set):** CSIB-155670 (Estimates),
155671 (PO Requisitions), 155673 (RMAs), 155674 (Opportunities), 155675 (Campaigns),
155676 (Recurring Vouchers), 155677 (Service Contracts), 155678 (ECN), 155679 (Purchase Orders),
155680 (Transfer Orders), 155681 (Delivery Orders), 155682 (Job Orders), 155683 (Service Orders),
155684 (Projects), 155685 / 155686 / 155687 (Production Schedules)
**Tree-component removal:** CSIB-159623 / 159624 / 159625 / 159626
**Deep defects:** CSIB-159418, 159423, 159468, 159473, 159524, 159558, 159560, 159719,
160905, 160909, 160910, 160956, 160957, 162059, 162062, 162101, 161878, 161900, 161905,
155879 (performance), 155880 (arrow navigation), 155906 (sub-collection grid binding type error),
CSIB-172185 (`RL_ShadowItemGridCol` bound to the wrong collection — object2 vs object4)

### What it actually was

Merging separate header/line/detail forms into a **single consolidated form per business entity**,
then making the sub-collection grid fully editable in place — add, maintain, delete, default,
validate — for ~17 entities. This is a coherent architectural pattern applied across the product's
entire transactional surface.

### Key skills I learned

- **Applying one pattern across ~17 entities** and keeping it consistent — the closest thing to
  architecture I had done at that point
- **Deliberate simplification** — CSIB-159623–159626, removing tree components; CSIB-162250,
  *"Remove unnecessary drilldown component against datagrid."* **Deleting things is design work.**
  I learned that a good migration removes complexity rather than porting it.
- **Component uplift** — CSIB-161147, upgrading the drilldown control across all consolidated
  forms
- **Master–detail state management** — the recurring hard case: creating a line *before* the
  header is saved (CSIB-160905, 160956, 160957, 159423, 159719). Defaulting, validation, and
  save-enablement all depend on parent state that does not exist yet.
- **Data-binding precision** — CSIB-155906 and CSIB-172185. In CSIB-172185 I identified a grid
  column bound to the wrong collection object (`object2` vs `object4`). That is reading the form
  definition like source code.
- **Performance awareness** — CSIB-155879, a consolidated form is heavier than the forms it
  replaced; consolidation has a cost
- **Keyboard/interaction completeness** — CSIB-155880, arrow navigation

### Hardest problem I struggled with

**Editing a sub-collection line before its parent header exists.** Look at how many tickets
circle this one problem: CSIB-160905 (related item data not brought up when creating a line
without saving the header), CSIB-160956 (error adding a blanket PO line without clicking Add),
CSIB-160957, CSIB-159423 (cannot input line data on a new blanket line), CSIB-159719 (error
saving header and line together without required data), CSIB-162059 / 162062 (U/M not required,
due date not defaulted). Every one is the same underlying question: **what is the valid
intermediate state of an unsaved parent–child pair, and when do defaults and validation fire?**

I did not solve that in one go. I solved it by grinding through a dozen manifestations until the
model was clear. That is honest and it is how hard problems actually get solved — but it also
tells me I should have stopped and modelled it explicitly earlier.

### My biggest contribution

I carried a single architectural pattern across ~17 business entities and **reduced** complexity
while doing it (tree removal, drilldown uplift, unnecessary component removal). And I found
binding-level root causes (CSIB-172185, CSIB-155906) that would have been reported as vague
"grid doesn't work" tickets by most people.

### Verdict

My first taste of applying **one design decision at product scale**. The direct bridge to §10.

---

## 10. Project: Code out of UI (COUI) — ChangePOStatusUtility & VendorInteractions

**Period:** 2026 (current, most senior work)
**Parent features:** CSIB-166006 (`IDS UX: Code out of UI - Form - ChangePOStatusUtility.ids`),
CSIB-165592 (`IDS UX: Code out of UI - Form Wash Up - VendorInteractions.ids`)

**Specifications I authored:** CSIB-166585 (ChangePOStatusUtility Specification),
CSIB-167015 (VendorInteractions Specifications)

**Story decomposition — deliberate API/UI split, my design:**

| Story                       | Ticket      | Layer |
| --------------------------- | ----------- | ----- |
| 1B RunProcess               | CSIB-166218 | UI    |
| 2A SetOldStatusEvent        | CSIB-166219 | API   |
| 3B RunBackgroundQueue       | CSIB-166220 | UI    |
| 4A GenerateReport           | CSIB-166222 | API   |
| 8A/9A GetDefaultEndValue    | CSIB-166242 | API   |
| 8B GetDefaultEndPoNumValue  | CSIB-166807 | UI    |
| 9B GetDefaultEndDateValue   | CSIB-166808 | UI    |
| 10A ValidateOffsetDeletion  | CSIB-174929 | API   |
| 11A ValidateAPPaymentDelete | CSIB-174931 | API   |

**Architecture work:** CSIB-170408 (create persistent staging table `tmp_change_po_status`),
CSIB-167387 (Permanent Filter API / CRUD API for primary collection), CSIB-167708 (Validator API),
CSIB-168526 (CRUD API for sub-collection), CSIB-168212 (**migrate `EnableWhen` from component
properties into IDO Data Rules**), CSIB-167393 (API Rework), CSIB-167394 (UI Rework),
CSIB-168589 (correct the IDO Entry Point name), CSIB-168676 (add missing component settings from
component classes), CSIB-168527 (`Unable to create IDO extension class CSI_Internal.MG.Vendor.SLPos`)

**Standards enforcement:** CSIB-168674 — *"Guideline Violation: each event to at most two
handlers per collection"*
**Review loops:** CSIB-167526 (Code Review Feedback), CSIB-170229 (Fix Review Feedback),
CSIB-169860 (my spec's CRUD API section was not clear enough for the QA test plan & automation)

**API test suite I designed** — a systematic negative matrix over insert × update × Email /
non-Email type × valid / invalid / empty:
CSIB-170257, 170330, 170331, 170358, 170438, 170442, 170443, 170464, 170513, 170514, 170528,
170535, 170536, 170804, 170815, 170927, 171109, 171167, 171168, 171237, 172487, 172685, 172686,
172793, 173058, 173059, 173060, 174555, 173861

### What it actually was

The **Code out of UI** initiative: move business logic out of form script and into the IDO tier —
CRUD APIs, validator APIs, permanent filters, IDO Data Rules — so behaviour is testable,
reusable, and not trapped in the UI. I own two forms end-to-end: specify, decompose, implement,
test, review.

### Key skills I learned

- **Writing specifications other people build and test against.** CSIB-166585 and CSIB-167015.
  CSIB-169860 is feedback that my spec was not clear enough for QA automation — I am now
  accountable for the *quality of my documents*, not only my code.
- **Decomposing a feature along the architectural seam.** Every story is explicitly A (API) or
  B (UI). That is not project-management bookkeeping; it is me enforcing the layer boundary
  through the work breakdown itself.
- **Declarative over imperative** — CSIB-168212, migrating `EnableWhen` from component properties
  into **IDO Data Rules**. Moving a rule from where it is *displayed* to where it is *true*.
  This is the deepest design idea I have applied so far.
- **API design as a first-class deliverable** — validator API, permanent filter API, CRUD API for
  a sub-collection; deciding what belongs in each
- **Schema design for process state** — CSIB-170408, a persistent staging table for a batch
  utility
- **Specification-based negative testing.** ~29 tickets. Not happy paths — an exhaustive matrix
  that found real defects: immutable fields (`Type`, `ContactDate`, `EnteredBy`) were updatable
  (CSIB-170514); email fields accepted on non-email records (CSIB-170358, 170528); a
  `bad_email` status accepted when it must be rejected (CSIB-171109); inconsistent attachment
  flags (CSIB-170438); empty Notes updating successfully (CSIB-170513); misleading response
  messages (CSIB-170815, 170927, 171167, 172487).
- **Enforcing guidelines on others' work** — CSIB-168674, citing a specific rule (at most two
  handlers per event per collection)

### Hardest problem I struggled with

**MGD-40464** — see §11. It belongs to this project and it is the hardest thing I have debugged.

Beyond that: the constant tension of COUI itself. Every rule I move out of the UI has to keep
behaving *identically* in the UI, while now also being correct when called directly by an API
with no UI at all. Two contracts, one implementation.

### My biggest contribution

**I am now upstream of other people.** I write the spec; QA writes tests against it; other
developers implement stories from it; I give review feedback and cite guideline violations. In
2022 I received fully-specified conversion tickets. In 2026 I produce the specification.

And the API test matrix is genuinely valuable work: ~29 real defects in validation and error
handling that would otherwise have reached customers as "the API let me save nonsense."

### Verdict

**This is my current level, and it is a real level change.** Not "I write good code" — "I decide
where code goes, prove it, and hold others to it."

---

## 11. Project: Mongoose Platform Defects (MGD) — the level marker

**Period:** 2025 – 2026
**Issues I raised against the platform itself:**

- **MGD-38538** — *AutoNumber support in the IDO tier for property DefaultValue* (a **feature
  proposal**, not a bug)
- **MGD-38621** — CRUD API does not apply `DefaultValue` when a read-only property is enabled via
  a DataRule on insert
- **MGD-40112** — a `Required` DataRule condition evaluates the request payload's `Modified` flag
  instead of the effective value, so a property present with `Modified=false` bypasses the
  required check and the insert fails with a raw database *"cannot be null"* error
- **MGD-40464** — *Method call RVAR write-back to a form variable does not notify variable
  dependents — a component whose Add/Details Form uses `V()` never re-resolves and right-click
  Details fails*

### Why this matters more than anything else in this file

These are filed against **Mongoose, the framework my product runs on** — not my own code. To file
them I had to understand the platform better than the platform's own documentation states.

### MGD-40464 in detail — my best piece of engineering work to date

What I did, in order:

1. **Isolated the divergence.** A `MethodCall` response with an `RVAR V(SomeVar)` parameter
   *stores* the returned value into the form variable but does **not** raise the variable-changed
   notification to that variable's registered dependents.
2. **Proved the value was stored.** Read the same variable from form script in the same event
   chain — it returns the correct value. So the store works; the notification does not. This
   single experiment cut the problem in half.
3. **Found a minimal, absurd workaround and understood *why* it works** — a value-identical
   self-assignment:
   ```vb
   ThisForm.Variables("RightClickFormVar").Value = ThisForm.Variables("RightClickFormVar").Value
   ```

   It changes nothing about the value. Its only effect is the notification side effect. I wrote
   exactly that reasoning in the ticket.
4. **Explained it by analogy to a documented parallel in the same framework** —
   `SetObjectProperty` (sets the value only) versus `SetObjectPropertyPlusModifyRefresh` (also
   marks modified and notifies dependents to refresh). The `RVAR` write-back appears to take the
   equivalent non-notifying path. I found the platform's own precedent for my hypothesis.
5. **Asked two precise design questions instead of demanding a fix** — should `RVAR` write-back
   notify, matching form script and `SETVARVALUES`? If not, what is the *supported* way to make a
   `V(...)`-based Add/Details Form re-resolve after a method call?
6. **Stated the architectural impact.** Every COUI-migrated form that resolves a right-click
   Details target through variables now needs a form-script line that reads as dead code — which
   contradicts the COUI guideline to minimise form script, and will be deleted in review or lost
   in migration.
7. **Recorded the exact environment** — Mongoose Web Client 2026.10.03, Build P#19492766.

### Key skills this demonstrates

- Root-cause analysis **one layer below my own product**
- Designing an experiment that halves the problem space (step 2)
- Refusing to accept a working workaround without understanding it (step 3)
- Using a framework's own documented behaviour as evidence (step 4)
- Writing for a **peer team** rather than a ticket queue — questions, not demands (step 5)
- Connecting a low-level defect to a **strategic initiative** (step 6)

### My biggest contribution

I turned "right-click Details is broken on my form" into a documented framework design question
with a repro, a proof, a workaround, an explanation, and an impact analysis. That report is
useful to the platform team even if I never touch the form again.

### Verdict

**This is the artefact that proves my current level.** If I only keep one thing from these five
years, keep MGD-40464 and the habit that produced it.

---

## 12. What actually changed in me, 2022 → 2026

| Axis                             | March 2022                                                         | August 2026                                                                                                                                                   |
| -------------------------------- | ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Input I work from**      | A fully specified ticket (`C#izer - Conversion - APQPCustUpdSp`) | A business need; I write the spec (CSIB-166585)                                                                                                               |
| **SOLID**                  | Can name the five principles                                       | Applied DI over factories across four folders (CSIB-57981/94/95, 58001); split interfaces for SRP (CSIB-59898); moved rules into IDO Data Rules (CSIB-168212) |
| **Layers I touch**         | C# middle tier only                                                | Schema → SP → C# IDO → REST/business API → Gen2/IDS form → mobile                                                                                        |
| **Testing**                | `UT: GetServiceUrl`                                              | ~29-ticket negative API matrix that found real validation defects                                                                                             |
| **Debugging depth**        | Fix my own code                                                    | Root-cause the framework (MGD-40464)                                                                                                                          |
| **Bug reports**            | "It doesn't work"                                                  | "Line 137, wrong variable, should be`@PEndInv`" (CSIB-69945)                                                                                                |
| **Scope of a decision**    | One method                                                         | ~17 business entities (§9); a product-wide initiative (§10)                                                                                                 |
| **Relationship to others** | Consume specs                                                      | Produce specs; review code; cite guideline violations (CSIB-168674)                                                                                           |
| **Written English**        | `UT：MassageParser` — full-width colon, "Massage" for "Message" | *"ContactDate default from CURDATE() CURTIME() fails to parse in ContactDateDefault (SLVendorInteractionDetails_IDS insert)"*                               |

### The five things I can genuinely claim

1. **Vertical range** across one large ERP: database schema to mobile UI.
2. **Root-cause precision** — my defining strength, evidenced from 2023 (line-level SQL) to 2026
   (framework notification paths).
3. **Design authority** — specifications, schema review/approval (CSIB-71492/71526), standards
   (CSIB-68424), code review feedback (CSIB-167526), guideline enforcement (CSIB-168674).
4. **Delivery discipline** — licences, permissions, help IDs, translations, manifests,
   documentation, knowledge transfer. I finish things.
5. **Written technical English** — measurably improved, on the record, over four years.

---

## 13. What is missing — read this part twice

1. **Depth without breadth.** 725 of 738 issues are in CSIB. Everything is SyteLine on Mongoose.
   There is **no evidence in four and a half years** of cloud, containers, CI/CD ownership, or a
   second language ecosystem. One `DevOps Review` ticket in 2023 (CSIB-68422) is the entire
   record. If I ever have to leave this product, most of my visible value does not travel with me.
2. **My thinking is not durable.** I have created **one** Confluence page in five years — my own
   profile page, February 2023. My best analysis, MGD-40464, is buried in a Jira ticket that
   nobody will search for in two years. **This is the cheapest fix available and the biggest limit
   on my influence.** I have solved problems (the unsaved parent–child state model in §9; the
   COUI API/UI split in §10) that the next person will have to rediscover from scratch.
3. **No record of leading anyone.** `Knowledge Transfer Recording` tickets are the closest thing.
   Nothing shows me mentoring, onboarding, or driving a change across teams.
4. **I solve hard problems by grinding, not by modelling.** §9 is the proof: a dozen tickets
   circling one question about unsaved parent–child state. I got there, but slowly. I should learn
   to stop after the second or third symptom and write the model down.
5. **Volume is still a habit.** 208 issues in 2025, many of them "column not fully shown" and
   "missing button icon". Necessary, but it is not what grows me any more.

---

## 14. Next 12 months — three moves, in order of leverage

1. **Write down what I already know.** Turn the COUI experience into a real design document:
   the API/UI story split, when a rule belongs in an IDO Data Rule versus a validator API, the
   unsaved parent–child state model, the notification traps (MGD-40464). I have now done COUI
   twice — ChangePOStatusUtility and VendorInteractions. **The third team to do it should read my
   page, not re-derive it.** This is one page of writing for a permanent increase in my visibility
   and leverage.
2. **Turn platform bug reports into platform contributions.** I already file MGD tickets the
   platform team must answer, and MGD-38538 shows I can propose a feature. Next step: ask to
   implement one. That moves me from "reports framework problems" to "improves the framework."
3. **Add one deliberate breadth area outside SyteLine.** One thing, deep enough to ship
   something. My depth is real; breadth is now the binding constraint.

---

## 15. One-paragraph answer to "what have I done?"

I started as someone who executed fully-specified stored-procedure conversions inside a single
layer of one ERP. I am now someone who writes the specification, decomposes it along the
architectural seam, moves business rules out of the UI into the right tier, designs the negative
test matrix that proves them, root-causes defects in the framework my product runs on, and holds
other engineers to the guidelines. Over four and a half years: 656 issues resolved, 158 raised,
one product understood from schema to mobile UI. The technical gap is no longer the problem. The
gap is that almost none of my thinking is written down anywhere anyone else can find it.

---

*Generated 2026-08-31 from infor.atlassian.net (Jira + Confluence). Every issue key above is real
and can be opened at `https://infor.atlassian.net/browse/<KEY>`.*

---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: 16108e5e-6e1a-40a4-9570-0bb6afe3ec89
exo__Asset_createdAt: 2026-04-27T20:03:15
exo__Asset_updatedAt: 2026-04-27T20:03:15
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Class]]"
exo__Asset_label: pmbok__AllDisjointClassesAxiom
exo__Class_superClass:
  - "[[exo__Asset]]"
exo__Asset_description: OWL axiom asset declaring 8 PMBOK lifecycle classes pairwise mutually disjoint — owl:AllDisjointClasses(pmbok__ProjectCharter, pmbok__ProjectStatusRecord, pmbok__ProjectClosureReport, pmbok__RiskItem, pmbok__IssueItem, pmbok__ChangeRequest, pmbok__Lesson, pmbok__Milestone). 28 unique pairwise owl:disjointWith assertions encoded в один axiom (per RFC v3 Ontology N3). Invariant — single asset cannot classify simultaneously as multiple lifecycle types. Implementation in M1.1 — Charter / StatusRecord / Closure / Lesson exist; Risk / Issue / CR / Milestone arrive в M2-M5 (axiom forward-declares их disjoint partition). Verification — test-write dual-classified instance must be blocked by future hook integration; до M1.2 hook update — semantic axiom, validation manual.
exo__Asset_relates:
  - "[[pmbok__ProjectClosureReport]]"
  - "[[pmbok__Lesson]]"
  - "[[4bd103cb-88ed-4a23-b51f-1d0afb166c6f|RFC pmbok-lifecycle v3]]"
---

## 8-Class Disjointness Matrix

| | Charter | StatusRecord | Closure | Risk | Issue | CR | Lesson | Milestone |
|---|---|---|---|---|---|---|---|---|
| **Charter** | — | ⊥ | ⊥ | ⊥ | ⊥ | ⊥ | ⊥ | ⊥ |
| **StatusRecord** | | — | ⊥ | ⊥ | ⊥ | ⊥ | ⊥ | ⊥ |
| **Closure** | | | — | ⊥ | ⊥ | ⊥ | ⊥ | ⊥ |
| **Risk** | | | | — | ⊥ | ⊥ | ⊥ | ⊥ |
| **Issue** | | | | | — | ⊥ | ⊥ | ⊥ |
| **CR** | | | | | | — | ⊥ | ⊥ |
| **Lesson** | | | | | | | — | ⊥ |
| **Milestone** | | | | | | | | — |

28 unique pairs (8×7/2). All asserted disjoint by single owl:AllDisjointClasses axiom.

## Members

- [[pmbok__ProjectCharter]] (M1 — exists)
- [[pmbok__ProjectStatusRecord]] (M1 — exists)
- [[pmbok__ProjectClosureReport]] (M1.1 — created with this axiom)
- pmbok__RiskItem (M2 — forward-declared)
- pmbok__IssueItem (M3 — forward-declared)
- pmbok__ChangeRequest (M5 — forward-declared)
- [[pmbok__Lesson]] (M1.1 — created with this axiom)
- pmbok__Milestone (M4 — forward-declared)

---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: e8180ce1-f7a6-4e49-85c6-4d127e650ee4
exo__Asset_createdAt: 2026-04-29T18:54:18+0500
exo__Asset_updatedAt: 2026-04-29T19:28:54+0500
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Property]]"
  - "[[exo__ObjectProperty]]"
exo__Asset_label: pmbok__RiskItem_realizedAsIssue
exo__Asset_description: Links a pmbok__RiskItem (когда status=Realized) к the spawned pmbok__IssueItem. Cardinality 0..N — single Risk может realize в multiple Issues over time. Reciprocal — pmbok__IssueItem_spawnedFromRisk (declares owl:inverseOf, completing the inverse pair as of M3.1).
exo__Property_domain: "[[pmbok__RiskItem]]"
exo__Property_range: "[[pmbok__IssueItem]]"
---

## Notes
- **owl:inverseOf:** [[pmbok__IssueItem_spawnedFromRisk]] — bidirectional inverse pair completed in M3.1 (2026-04-29). Forward direction Risk→Issue declared here; reverse Issue→Risk declared on `pmbok__IssueItem_spawnedFromRisk`. OWL reasoner derives the missing direction from either declaration.
- **Range materialized:** as of M3.1 `pmbok__IssueItem` class exists; range wikilink resolves cleanly through validate-wikilinks hook.

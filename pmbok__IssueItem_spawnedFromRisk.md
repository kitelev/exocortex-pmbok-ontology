---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: 7478b581-9a84-4b70-b703-119e23756aea
exo__Asset_createdAt: 2026-04-29T19:28:54
exo__Asset_updatedAt: 2026-05-03T10:30:00
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Property]]"
  - "[[exo__ObjectProperty]]"
exo__Asset_label: pmbok__IssueItem_spawnedFromRisk
exo__Asset_description: Links a pmbok__IssueItem back to the pmbok__RiskItem from which it was realized (когда Risk status=Realized triggers Issue spawn). Cardinality 0..1 — issue may originate from a risk OR be raised directly. Reciprocal of pmbok__RiskItem_realizedAsIssue (declares owl:inverseOf, completing the inverse pair from M2.1).
exo__Property_domain: "[[pmbok__IssueItem]]"
exo__Property_range: "[[pmbok__RiskItem]]"
exo__Property_cardinality: "[[exo__PropertyCardinalitySingle]]"
exo__Property_severity: "sh:Violation"
---

## Notes
- **owl:inverseOf:** [[pmbok__RiskItem_realizedAsIssue]] — bidirectional inverse pair. SPARQL queries can traverse Risk→Issue via `pmbok:RiskItem_realizedAsIssue` или Issue→Risk via `pmbok:IssueItem_spawnedFromRisk`; OWL reasoner derives missing direction.
- **Cardinality 0..1:** an issue may exist independently of any risk (raised directly, not from RiskItem realization). When linked, RiskItem._status must be `pmbok__RiskStatusRealized`.

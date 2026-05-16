---
exo__Asset_isDefinedBy: "[[58df7855-d5fc-4f7c-9fa5-d909a1749b7e]]"
exo__Asset_uid: 72213088-ba38-4a5e-89eb-ba020f2b5d97
exo__Asset_createdAt: 2026-04-29T21:31:16
exo__Asset_updatedAt: 2026-05-03T10:30:00
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Property]]"
  - "[[exo__DatatypeProperty]]"
exo__Asset_label: pmbok__ProjectCharter_baselineFrozenAt
exo__Asset_description: Timestamp когда Charter baseline (Scope+Schedule+Cost+Quality) frozen — point-in-time snapshot после которого изменения требуют formal pmbok__ChangeRequest. Cardinality 0..1 (absent = baseline NOT frozen, CRs accepted без guard). Range xsd:dateTime. Set by /pmbok-baseline-freeze skill; --force-refreeze appends prior value к _baselineFrozenAtHistory array. Per RFC v3 Phase 6 Charter additions.
exo__Property_domain: "[[pmbok__ProjectCharter]]"
exo__Property_range: "xsd:dateTime"
exo__Property_cardinality: "[[exo__PropertyCardinalitySingle]]"
exo__Property_severity: "sh:Violation"
exo__Asset_relates:
  - "[[4bd103cb-88ed-4a23-b51f-1d0afb166c6f|RFC pmbok-lifecycle v3]]"
---

# pmbok__ProjectCharter_baselineFrozenAt

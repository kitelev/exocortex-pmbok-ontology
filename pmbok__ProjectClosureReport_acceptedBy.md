---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: 81fcb3ca-e433-421c-aa72-868d5fbbad17
exo__Asset_createdAt: 2026-04-27T20:03:15
exo__Asset_updatedAt: 2026-05-03T10:30:00
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Property]]"
  - "[[exo__ObjectProperty]]"
exo__Asset_label: pmbok__ProjectClosureReport_acceptedBy
exo__Asset_description: Person / agent who formally accepted closure (sponsor или accountable stakeholder). Semantic — prov:wasAssociatedWith (Activity → Agent — НЕ wasAttributedTo per RFC v3 Ontology N9 — PROV-O Entity ⊥ Activity disjoint, ClosureReport ∈ Activity therefore wasAttributedTo invalid). superProperty declaration документирует RDF-level alignment с PROV-O. Cardinality 1 (required). Range ims__Person.
exo__Property_domain: "[[pmbok__ProjectClosureReport]]"
exo__Property_range: "[[ims__Person]]"
exo__Property_cardinality: "[[exo__PropertyCardinalitySingle]]"
exo__Property_severity: "sh:Violation"
exo__Property_superProperty:
  - "[[prov__wasAssociatedWith]]"
---

---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: b86cb11b-6427-4451-96a8-3923a559f90c
exo__Asset_createdAt: 2026-04-27T20:03:15+0500
exo__Asset_updatedAt: 2026-05-03T10:30:00+0500
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Property]]"
  - "[[exo__DatatypeProperty]]"
exo__Asset_label: pmbok__ProjectClosureReport_acceptedAt
exo__Asset_description: Formal acceptance moment — sponsor / accountable agent signed off deliverables. Separate property от _closureDate per RFC v3 Ontology N5 (acceptance ≠ administrative closure event). Declares owl:equivalentProperty dcterms:dateAccepted (formal RDF-level equivalence — Dublin Core Terms vocabulary). superProperty fallback declaration via dcterms:dateAccepted документирует weaker rdfs:subPropertyOf relation до hook whitelist owl__equivalentProperty в M1.2. Cardinality 1 (required). Range xsd:dateTime.
exo__Property_domain: "[[pmbok__ProjectClosureReport]]"
exo__Property_range: "xsd:dateTime"
exo__Property_cardinality: "[[exo__PropertyCardinalitySingle]]"
exo__Property_severity: "sh:Violation"
exo__Property_superProperty:
  - "[[dcterms__dateAccepted]]"
---

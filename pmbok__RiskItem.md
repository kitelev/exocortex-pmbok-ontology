---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: ff1b9be3-9ffd-4d15-aa73-7e8ed94fe9bf
exo__Asset_createdAt: 2026-04-29T18:54:18+0500
exo__Asset_updatedAt: 2026-04-29T18:54:18+0500
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Class]]"
exo__Asset_label: pmbok__RiskItem
exo__Asset_description: PMBOK Risk Management — discrete risk register entry tracking a potential project event with status, probability, impact и optional mitigation summary. Living artifact (status transitions Open→Mitigated→Realized→Closed). prov:Entity-style placeholder. Disjoint with pmbok__IssueItem (M3 territory) — Risk = potential, Issue = realized; if Risk realized, _realizedAsIssue links к spawned IssueItem.
---

# pmbok__RiskItem

## Notes
- **Disjoint placeholder для M3:** instances of pmbok__RiskItem MUST NOT be instances of pmbok__IssueItem. Реализация через `owl:disjointWith pmbok:IssueItem` будет добавлена при создании IssueItem class в M3.
- **prov:Entity alignment:** RiskItem semantically a `prov:Entity` (potential entity describing project risk state). Wikilink не материализован (prov__Entity ассет ещё не создан в vault) — placeholder note для future RDF export.
- **`_realizedAsIssue` inverse:** при создании M3 ассета `pmbok__IssueItem_spawnedFromRisk` объявить `owl:inverseOf pmbok:RiskItem_realizedAsIssue` (reciprocal).
- **Frontmatter exemplar для instance:**
  ```yaml
  exo__Instance_class:
    - "[[pmbok__RiskItem]]"
  pmbok__RiskItem_project: "[[<project-uid>|<project label>]]"
  pmbok__RiskItem_status: "[[pmbok__RiskStatusOpen]]"
  pmbok__RiskItem_probability: "[[pmbok__RiskProbabilityMedium]]"
  pmbok__RiskItem_impact: "[[pmbok__RiskImpactHigh]]"
  pmbok__RiskItem_mitigationSummary: "Brief mitigation strategy text"
  ```

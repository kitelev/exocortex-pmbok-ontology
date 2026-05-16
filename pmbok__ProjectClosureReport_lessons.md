---
exo__Asset_isDefinedBy: "[[!pmbok]]"
exo__Asset_uid: 8fdfa0d8-a52f-4049-8f60-a2e3dcbb6d88
exo__Asset_createdAt: 2026-04-27T20:03:15
exo__Asset_updatedAt: 2026-05-09T18:55:52
exo__Asset_createdBy: "[[de20a3f1-7483-4714-ab28-b45f5cf02c76|ExoAssistant]]"
exo__Instance_class:
  - "[[exo__Property]]"
  - "[[exo__ObjectProperty]]"
exo__Asset_label: pmbok__ProjectClosureReport_lessons
exo__Asset_description: DEPRECATED per RFC d9dda65f (pmbok-artifacts v3.2). Parent→children UWI violation — Closure держал wikilinks-array на все дочерние Lessons. Заменяется inverse SPARQL: ?lesson pmbok:Lesson_closureReport ?closure . Consolidated references к pmbok__Lesson instances extracted during или после project closure. /pmbok-close skill auto-calls /pmbok-lessons sweep (Phase M6 enhancement). Cardinality 0..N. Range pmbok__Lesson.
exo__Property_domain: "[[pmbok__ProjectClosureReport]]"
exo__Property_range: "[[pmbok__Lesson]]"
exo__Asset_legacyValidationException: true
---

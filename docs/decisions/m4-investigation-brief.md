# M4 Investigation Brief

## Product Slice
US-06 Preserve Progress Between Sessions

## Trace to Product Work
"Given a learner has saved a practice progress, when the learner leaves and later returns using the same authenticated account, then the system retrieves the learner's saved progress."
This story is important to investigate because learners need to be able to return to their practice activities after an interruption without losing their progress. However, the backlog identifies unresolved questions about learner authentication, session management, and how saved progress should be retained.

## Initial Design Question
**Question type:** Data / State

How should the program save and retrieve a learner’s practice progress so that the learner can leave the application and return later using the same authenticated account without losing progress?

## Why This Question Matters
Coding before answering this question could create rework because the application might use a saving method that does not properly preserve a learner’s progress between sessions.

## Planned Evidence
- ERD / relationship model
- Field or state table

## Why This Evidence Is a Reasonable Starting Point
A relationship model will identify how learner accounts, practice sessions, and saved progress should relate to one another. A field/state table will determine what details will be saved, and what information is retrieved when a learner returns.

## Studio Check
During the DataMan Design Studio, record whether the evidence actually answered the question, whether you needed different evidence, and what new question emerged.

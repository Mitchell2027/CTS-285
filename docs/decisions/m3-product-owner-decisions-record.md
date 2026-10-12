# M3 Product Owner Decision Record

## Scenario
StudyTrack release planning under constrained capacity.

## Round 1 — Capacity 13
- ST-01: Create a study task (3 pts)
- ST-02: Mark a study task complete (2 pts)
- ST-03: Recover a missed task (3 pts)

**Why this release slice was defensible:**
Create a study task is a core behavior that should exist first and matters most because the students' need is to plan a task. Depending if the task is done, a student can mark it complete or recover a missed task. These decisions are clear enough to commit.

**One intentional deferral and why:**
I intentionally deferred the color theme decision because it is a design choice that should be decided in the future.

## Complication
Capacity dropped from 13 to 10 points. Keyboard accessibility testing revealed that task entry cannot reliably be completed with keyboard navigation, so ST-04 became release-critical.

## Revised Release Slice — Capacity 10
- ST-01: Create a study task (3 pts)
- ST-02: Mark a study task complete (2 pts)
- ST-03: Recover a missed task (3 pts)
- ST-04: Keyboard-accessible task entry (2 pts)

### Removed after complication
- None

### Added after complication
- ST-04: Keyboard-accessible task entry

**What changed and why:**
I changed to full capacity and added the keyboard accessible task entry. The plan changed because accessibility testing identified a problem with keyboard navigation. I prioritized keyboard-accessible task entry because the issue must be addressed before release.

**Tradeoff accepted:**
The tradeoff is that students will have fewer reporting and personalization features in this release, but the app will provide essential planning and recovery features with improved accessibility.

## Transfer to DataMan
Before finalizing your DataMan backlog, review whether any item is high value but not ready, depends on unresolved work, consumes disproportionate effort, or should move because it reduces risk or unlocks other work.

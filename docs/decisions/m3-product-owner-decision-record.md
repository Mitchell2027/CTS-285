# M3 Product Owner Decision Record

## Scenario
StudyTrack release planning under constrained capacity.

## Round 1 — Capacity 13
- ST-01: Create a study task (3 pts)
- ST-02: Mark a study task complete (2 pts)
- ST-03: Recover a missed task (3 pts)
- ST-04: Keyboard-accessible task entry (2 pts)

**Why this release slice was defensible:**
Create a study task is a core behavior that should exist first and matters most because the students' need is to plan a task. Depending if the task is done, a student can mark it complete or recover a missed task.  I also included keyboard-accessible task entry because students need to be able to create tasks reliably using keyboard navigation. These decisions are clear enough to commit.

**One intentional deferral and why:**
I intentionally deferred the color theme feature, because it is a enhancement that does not directly support the students' primary needs of creating, completing, or recovering study tasks. I prioritized the essential study-planning features because they provide greater value to students in this release.

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
- None

**What changed and why:**

The capacity dropped from 13 to 10 points, but I kept ST-01, ST-02, ST-03, and ST-04 in the release because they support essential tasks and keyboard accessibility. Since these stories total 10 points, they fit within the revised capacity and did not need to change because they already addressed the most important user needs.

**Tradeoff accepted:**
The tradeoff I accepted was using the full capacity for essential study-planning features and keyboard accessibility, leaving no capacity for additional features or enhancements in this release.

## Transfer to DataMan
Before finalizing your DataMan backlog, review whether any item is high value but not ready, depends on unresolved work, consumes disproportionate effort, or should move because it reduces risk or unlocks other work.

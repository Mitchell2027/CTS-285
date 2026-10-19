# DataMan Product Backlog

## Sources

This backlog uses these files from my repository:

- `docs/requirements.md`
- `docs/decisions/m3-backlog-triage-record.md`
- `docs/decisions/m3-product-owner-decision-record.md`

I revised `docs/requirements.md` after Module 2 in a resubmission on canvas.

## Priority Order

1. US-01 Immediate Answer Feedback
2. US-02 Select and play supported games
3. US-03 Display Game Results
4. US-04 Start, Continue, and Complete Practice
5. US-05 Browser-based application
6. US-06 Preserve Progress between session
7. US-07 Support Different Devices
8. US-08 Store and Retrieve Inputs
9. US-09 Retry after Incorrect Response
10. US-10 Parent/teacher Activity Summary

## Stories
-----------------------
### US-01 — Immediate Answer Feedback

**Requirement ID:** FR-02

**User Story:** As a learner, I want to know whether my submitted answer is correct or incorrect so that I can respond appropriately during practice.

**Acceptance Criteria:**

- Given a learner submits a correct answer during a practice session, when the system evaluates the answer, then the system displays
feedback indicating if the answer is correct.
- Given a learner submits an incorrect answer during a practice session, when the system evaluates the answer, then the system displays feedback indicating the answer is incorrect.
  
**Relative Effort:** S — This story requires less effort than stories involving saved progress, input storage, or activity reporting 
because it focuses on providing feedback through the existing answer-checking flow.

**Dependency / Constraint:**  Requires an answer-checking flow. Learners must be able to understand the feedback.

**Priority:** 1

**Readiness:** Move Forward

**Priority Rationale:** This is a high-value, low-effort item with no dependency. 
The instructor stakeholder explicitly requires immediate answer feedback for the first usable release.
--------------------------

### US-02 - Select and play a game option

**Requirement ID:** FR-01 

**User Story:** As a learner, I want to select and play different games so that I can practice arithmetic 
activities available in DataMan.

**Acceptance Criteria:**

- Given the learner can play a supported game, when the learner selects an available option, then
the application opens that practice activity.

**Relative Effort:**  M — This story requires more effort than basic answer feedback because it
must allow learners to access and start the supported games.

**Dependency / Constraint:** The game options documented in the DataMan Manual must be identified in the application's 
game selection interface.

**Priority:** 2

**Readiness:** Move Forward

**Priority Rationale:** Selecting and playing supported games is essential to DataMan's core arithmetic-practice purpose. 
Learners must be able to access the activities the application provides.
-----------------------------
### US-03 - Display Game Results

**Requirement ID:** FR-05

**User Story:** As a learner, I want to see my results after completing a game so that I can
understand my performance.

**Acceptance Criteria:**

- Given the learner completes a game, when the system gathers the score, then the results of the corresponding
 game is displayed.

**Relative Effort:** M — This story requires more effort than basic answer feedback because it must track 
and display the score, number of tries, and number of ticks after a game is completed.

**Dependency / Constraint:** The game must track the score, number of tries, and number of ticks from the game.
Confirming how each game calculates its score.

**Priority:** 3

**Readiness:** Move Forward

**Priority Rationale:** This story allows learners to understand their performance after completing a game. Displaying the score, number of tries, and number of ticks helps learners review the results of their practice activities.
-----------------------------
### US-04 -  Start, Continue, and Complete Practice

**Requirement ID:** NFR-03

**User Story:** As a learner, I want to start, continue, and complete a practice activity so that I can work through 
the activity from beginning to end.

**Acceptance Criteria:**

- Given the learner can start an available practice activity, when the learner proceed through the activity according
to its documented rule, then the system indicates when the activity is complete.

**Relative Effort:**  M — This story requires more effort than basic browser access because it must support the 
practice activity from beginning to completion according to the game's rules.

**Dependency / Constraint:** The selected game must have its practice flow and completion conditions 
defined im the DataMan Manual.

**Priority:** 4

**Readiness:** Move Forward

**Priority Rationale:** Starting, progressing through, and completing practice are essential to the 
application's core purpose. This story supports the learner's ability to use the games rather than merely
view the game options.
-----------------------------
### US-05 - Browser-based application

**Requirement ID:** NFR-01

**User Story:** As a learner, I want to access DataMan through a web browser so that I can use the application
without needing to install a separate desktop application.

**Acceptance Criteria:**

- Given a learner has access to a supported web browser, when the learner accesses the application, 
then the application loads and is available for use.

**Relative Effort:** S — This story requires less effort than stories involving saved progress 
or activity reporting because it focuses on making the application accessible through a web browser.

**Dependency / Constraint:**  The application must be accessible through a web browser. The 
browser-based experience should be understandable without requiring a printed manual.

**Priority:** 5

**Readiness:** Move Forward

**Priority Rationale:** Browser-based access is necessary to deliver the modernized DataMan
experience identified by stakeholders. This supports the project's intended delivery approach.
-----------------------------
### US-06 — Preserve Progress Between Sessions

**Requirement ID:** FR-03

**User Story:** As a learner, I want my saved practice progress to be available when I return so that I can continue after 
an interruption.

**Acceptance Criteria:**

- Given a learner has saved a practice progress, when the learner leaves and later returns using the same authenticated
  account, then the sytem retrieves the learner's saved progress.

**Relative Effort:** L — This story requires more effort than most other stories because it depends on learner identity,
session management, and retrieving saved practice progress.

**Dependency / Constraint:** The system will need an authenticated identity approach to associate with saved progress. 

**Priority:** 6

**Readiness:** Refine

**Priority Rationale:** High value because it allows learners to resume practice after interruptions without losing progress.
However, unresolved learner identity and session management require refinement before implementaion.

-----------------------------
### US-07 - Support Different Devices

**Requirement ID:** NFR-04

**User Story:** As a learner, I want to complete practice activities on supported devices so that
I can use DataMan in different learning environments.

**Acceptance Criteria:**

- Given a learner accesses the application on a supported device, when the learner starts a
supported practice activity, then the learner can interact with the activity.
- The supported device types include school Chromebooks, phones, tablets, and home computers.

**Relative Effort:** M — This story requires more effort than basic answer feedback because
practice activities must remain usable across the different device types identified in the requirements.

**Dependency / Constraint:** The application must support completing practice sessions on the device.
Browser access is also required by browser-based application requirements.

**Priority:** 7

**Readiness:** Move Forward

**Priority Rationale:** Learners use DataMan in multiple environments, including school and home.
Supporting the identified device types makes the application accessible across those environments
and helps learners complete their practice activities.
-----------------------------
### US-08 - Store and Retrieve Inputs

**Requirement ID:** FR-04

**User Story:**  As a learner, I want to store and retrieve input values so that I can use
previously entered problems during supported practice activities.

**Acceptance Criteria:**

- Given a learner enters input values for a supported practice activity, when the 
learner stores those values, then the system retains the values for later use.
- Given previously stored input values are available, when the learner requests to retrieve
them during a supported practice activity, then the system makes the stored values available for use.

**Relative Effort:** M — This story requires more effort than basic answer feedback
because it must store input values and make the previously stored values available during supported practice activities.

**Dependency / Constraint:** The system must support input storage and retrieval for applicable games and practice activities. 

**Priority:** 8

**Readiness:** Move Forward

**Priority Rationale:** Input storage and retrieval supports the Memory Bank capability described in the DataMan Manual. 
It allows learners to reuse previously entered problems rather than entering the same values again. This supports 
repeated practice using stored inputs.
-----------------------------
### US-09 - Retry after Incorrect Response
**Requirement ID:** FR-02

**User Story:** As a learner, I want to retry after submitting an incorrect answer when the game's 
rules allow another attempt so that I can continue practicing and respond to the feedback.

**Acceptance Criteria:**

- Given a learner submits an incorrect answer during a supported practice activity, when the system evaluates the answer, then the same problem is still available to answer.

**Relative Effort:**  S — This story requires less effort than stories involving saved progress 
or input storage because it focuses on allowing another attempt according to the selected game's rules.

**Dependency / Constraint:** This story depends on immediate answer feedback because the system must evaluate submitted answers and provide immediate feedback before the learner can respond to an incorrect answer. Retry behavior must also follow the rules of the selected game.

**Priority:** 9

**Readiness:** Refine

**Priority Rationale:** Retry behavior can help learners continue practicing after an incorrect response.
However, the number of permitted attempts and the next step after an incorrect answer must be verified 
against the rules of each applicable game before implementation.
-----------------------------
###  US-10 - Parent/teacher Activity Summary
**Requirement ID:** FR-06

**User Story:** As an authorized parent or teacher, I want to view a learner's practice activity
and progress so that I can understand what the learner has practiced and whether progress is occurring.

**Acceptance Criteria:**

- Given an adult is authorized to view a learner's information, when the adult requests the learner's
practice information, then the system provides the available activity and progress information for that learner.

**Relative Effort:**  M — This story requires more effort than basic practice features because it must associate 
activity and progress information with the correct learner and restrict access to authorized adults.

**Dependency / Constraint:** The system must establish an authenticated identity approach to associate activity and progress information with the correct learner. Access must be restricted to authorized parents or teachers.

**Priority:** 10

**Readiness:** Refine

**Priority Rationale:** Parents and teachers need information about learner activity and progress to understand
whether practice is occurring and whether progress is being made.
-----------------------------

## Open Questions Carried Forward

- **Q-01** US-06 — How should a learner be identified and authenticated when returning to a saved practice session?
- **Q-02** US-10 — What specific practice activity and progress information should authorized parents or teachers be able to view?
- **Q-03** US-06 — Should learners have a manual save option in addition to automatic saving?
- **Q-04** US-06 and US-10 — How long must saved learner practice states and progress information be retained?

## Revisions After Triage and Release Planningx

- US-06 — Preserve Progress Between Sessions: Retained as a high-value requirement but marked Refine because learner identity and 
session management remain unresolved. Source: docs/decisions/m3-backlog-triage-record.md.
- US-01 — Immediate Answer Feedback: Retained as the first priority because it provides essential feedback with low effort. 
Source: docs/decisions/m3-product-owner-decision-record.md.

# DataMan Requirements Register

## Project Context

The project will be a web-based version of the original DataMan calculator that provides an arithmetic practice experience.
The primary users are learners who wants math practice and adults, such as teachers or parents, who needs to check the learners'
activity and progress. The project is intended to be accessible through a browser, without the need of a printed manual, and
more reliable when learners pause or leave and later return to their practice.

## Evidence Notes

- **E-01 — Source:** DataMan manual
  **Evidence:** DataMan provides an arithmetic practice experience in which learners answer math questions and receive feedback
  on their answers.

- **E-02 — Source:** Elicitation case 
  **Evidence:**  Stakeholders want the modernized DataMan experience to work reliably in a web browser, be understandable without
  a printed manual, and avoid unnecessary navigation.

- **E-03 — Source:** Elicitation case
  **Evidence:**  Teachers report that learners may pause practice and return later, creating a need for saved practice state to
remain available after leaving the application.

- **E-04 — Source:** Elicitation Case  
  **Evidence:**  Learners may use DataMan on school Chromebooks, phones, tablets, and home computers, and some sessions may be
interrupted before the learner intentionally exits or signs out.

## Functional Requirements

### FR-01
**Requirement:** The system must allow a learner to start an arithmetic practice session.
**Source/Rationale:** DataMan provides an arithmetic practice experience for learners.

### FR-02
**Requirement:** The system must provide feedback indicating whether a learner's submitted answer is correct or incorrect. 
**Source/Rationale:** The case states that learners need feedback during arithmetic practice so they can understand the result
of their submitted answers.

### FR-03
**Requirement:** The system must preserve a learner's saved practice progress between authenticated sessions.
**Source/Rationale:** Teachers report that learners may leave practice and return later, creating a need for saved progress to 
remain available. 

### FR-04
**Requirement:** The system must automatically save the learner's current practice state after each submitted answer. 
**Source/Rationale:** Sessions may be interrupted before a learner intentionally exits or signs out, so saving after each submitted answer reduces the risk of losing recent practice progress. 

### FR-05
**Requirement:** The system must allow a learner to resume practice from the most recently saved practice state.
**Source/Rationale:** Learners may pause practice and return later, so the saved state must be usable when they return.

### FR-06
**Requirement:** The system must provide authorized adults with understandable information about a learner's practice activity and progress.
**Source/Rationale:** Adults want to understand what learners practiced and whether progress is occurring.

## Non-Functional Requirements

### NFR-01
**Requirement:** The system must be accessible through a web browser.  
**Source/Rationale:** Stakeholders define the modernized experience by requiring reliable browser-based access.

### NFR-02
**Requirement:** The application must provide an understandable practice experience that does not require a printed manual for normal practice activities.
**Source/Rationale:** Stakeholders stated that the modernized experience should be understandable without a printed manual.

### NFR-03
**Requirement:** The application must minimize unnecessary navigation steps required to start, continue, and complete practice activities.
**Source/Rationale:** Stakeholders stated that the modernized experience should avoid making learners navigate unnecessary screens.

### NFR-03
**Requirement:** The application must support learner access from commonly used devices, including school Chromebooks, phones, tablets, and home computers.
**Source/Rationale:** Teachers identifies these devices as environments in which learners may use DataMan.

## Open Questions / Assumptions

- **Q-01:** How should a learner be identified and authenticated when returning to a saved practice session?
- **Q-02:** What specific practice activity and progress information should authorized parents or teachers be able to view?
- **Q-03:** Should learners have a manual save option in addition to automatic saving?
- **Q-04:** How long should saved learner practice states and progress information be retained?

## Final Quality Check

Before submitting, confirm that each requirement is:

- [x] Clear enough for another team member to interpret consistently.
- [x] Supported by evidence, a stakeholder need, or a confirmed project constraint.
- [x] Testable or verifiable later.
- [x] Solution-neutral enough for this stage of the project.
- [x] Focused on one main capability or quality.
- [x] Classified correctly as functional or non-functional.

Also confirm:

- [x] At least four functional requirements are included.
- [x] At least three non-functional requirements are included.
- [x] Every confirmed requirement has a source/rationale.
- [x] Open questions and assumptions are separated from confirmed requirements.
- [x] The simulation decision record is saved at `docs/decisions/m2-elicitation-decision-record.md`.
- [x] This file is saved as `docs/requirements.md`, committed, and synced to GitHub.

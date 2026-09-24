# M2 Elicitation Decision Record

## Investigation Path
1. What does “modern” need to mean from a user perspective?
   Evidence revealed: Stakeholders say modern means the experience should work reliably in a browser, be understandable without a printed manual, and avoid making the learner navigate unnecessary screens. They do not specify a visual style or framework.
2. What exactly do stakeholders mean by “students shouldn’t lose their work”?
   Evidence revealed: Teachers report that students may pause practice and return later. They want a learner’s saved practice state to remain available after leaving and returning to the application.
3. What do parents or teachers need to understand about learner activity?
   Evidence revealed: Adults want to understand what the learner practiced and whether progress is occurring, but stakeholders have not yet agreed on a detailed reporting dashboard.

## Initial Position
**Supported evidence:**
A web-based application to implement the Dataman original story. A learner should be able to pause the practice during a session and exit the application with their session saved to return for later use. A dashboard to track a users progress and display the learners practice.

**Remaining uncertainty:**
How simple should the webpage be? Is automatic or manual saving necessary during practice sessions? How can parent/educators access a specific user's progress?

**Likely functional requirement:**
The system must allow a user to save the current practice.
The system must preserve record of user's progression.

**Likely non-functional requirement / quality constraint:**
The web application allows a user to return to their saved practice after exiting the application.

**Assumption or proposed solution I am not treating as confirmed:**
Flask will be used to implement a modern web-based software is the proposed solution.

**Why my initial position is defensible:**
My initial position is defensible because Stakeholders want a Dataman web-based application. Which has a math practice that learners can save to avoid interruptions and record progression for their adult peers to review.

## Complication
Students may use DataMan on school Chromebooks, phones, tablets, and home computers. Some sessions may be interrupted before intentional sign-out.

**What this affects:**
This new information affect how practice session are saved.

**What I revised, if anything:**
I will revise that the users must save the practice.

**Final decision and reasoning:**
I will revise the system must save automatically after a learner has answered a question in the practice session. If the practice is interrupted or exited, the learner can return to the last question answered since the session was saved.

## Next Project Action
Use this evidence to update the DataMan Requirements Register and preserve any unresolved questions as open assumptions or follow-up items.

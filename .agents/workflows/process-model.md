---
description: Generate a Mermaid flowchart of a current-state or future-state business process from a BA elicitation description
---

# 1. Read Project Context
- Read `BA_Project_Checkpoint.md` — In-Scope items and business problem.
- Check `02_Elicitation_and_Collaboration/` for any existing process notes or transcripts that describe the process.

# 2. Define the Process — One Question at a Time
- **Q1:** "What is the name of the process we are modelling?" (e.g., "Month-End Close", "Order Fulfillment", "Contract Approval")
- **Q2:** "Are we modelling the **current state** (as-is) or the **future state** (to-be)?"
- **Q3:** "Who are the actors or roles involved in this process?" (e.g., Finance Team, System, External Client)
- **Q4:** "Walk me through the process steps in sequence. Describe each step briefly — I will convert them into the diagram."
- (After BA describes steps) **Q5:** "Are there any decision points — places where the process branches into different paths depending on a condition?"
- **Q6:** "Are there any steps that happen in parallel rather than in sequence?"

# 3. Generate the Process Model
Create `02_Elicitation_and_Collaboration/Process_Model_[ProcessName]_[AsIs|ToBe]_v1.md` containing:

1. A **Mermaid flowchart** using `flowchart TD` format:
   - Use `subgraph` to group steps by actor/swimlane
   - Use diamond nodes `{Decision}` for branching points
   - Use `-->|condition|` syntax for labelled decision paths
   - Use `&` or parallel notation for concurrent steps where applicable

2. A **Process Narrative** below the diagram:
   - Step-by-step description in plain English
   - List of key decision points and their conditions
   - Known pain points (if current-state) or improvement intent (if future-state)

3. A **Gap / Issue Note** (if current-state):
   - List any inefficiencies, bottlenecks, or compliance risks observed in the process description

# 4. Inform the BA
- "Your Process Model is at `02_Elicitation_and_Collaboration/Process_Model_[Name]_[AsIs/ToBe]_v1.md`."
- "If you modelled the current state, run `/process-model` again to model the future state and compare."

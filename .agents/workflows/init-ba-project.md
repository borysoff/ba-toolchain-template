---
description: Initialize a new Business Analysis project through conversational extraction
---

# 1. Start Q&A Session
Agent Initialization:
- Open `BA_Project_Checkpoint.md` to begin storing context.
- Tell the BA: "Welcome to the Self-Extracting BA Initialization Workflow. I will ask you a series of contextual questions to scaffold the environment. Let's start with the basics."
- Ask questions ONE AT A TIME based on the sections in `BA_Project_Checkpoint.md`. Do not overwhelm the user. Do not move to the next section until you have captured the required information.

# 2. Iterative Documentation
- As the BA answers, dynamically update `BA_Project_Checkpoint.md` in the background. Address them conversationally while doing so.
- Sections to cover:
  1. Identity & Baseline (Name, Domain, Problem)
  2. Stakeholders & Constraints
  3. High-Level Scope
  4. Methodological Tailoring

# 3. Knowledge Area Scaffolding
- When arriving at Section 4, ask the BA: "Based on what we've discussed, which of the 6 BABOK Knowledge Areas should we scaffold for this project? I can suggest the required ones or generate all of them."
- Once confirmed by the BA, check the boxes in `BA_Project_Checkpoint.md`.
- Based on the checked boxes, create the corresponding folders in the root directory:
  - `01_Planning_and_Monitoring`
  - `02_Elicitation_and_Collaboration`
  - `03_Requirements_Life_Cycle_Management`
  - `04_Strategy_Analysis`
  - `05_Requirements_Analysis_and_Design_Definition`
  - `06_Solution_Evaluation`

# 4. Finalization
- Inform the BA that the scaffold is complete and the `BA_Project_Checkpoint.md` is initialized.
- Remind the BA they can invoke specialized skills located in the `.agents/skills` folder (e.g., `/ifrs15-auditor` if placed there) to continue work within the generated Knowledge Areas.

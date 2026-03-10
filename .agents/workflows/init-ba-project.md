---
description: Initialize a new Business Analysis project through conversational extraction
---

# 1. Preparation & Document Ingestion
Agent Initialization:
- Create a folder named `00_Preparation` in the project root if it doesn't exist.
- Tell the BA: "Welcome to the Self-Extracting BA Initialization Workflow. To save time, please place any existing project documents (like a Project Charter, SOW, or Emails) into the `00_Preparation` folder."
- Tell the BA: "Let me know when you have placed the files there, or tell me if we are starting from scratch."
- Wait for the BA's confirmation.

# 2. Context Analysis 
- If the BA placed files in `00_Preparation`, use your tools (like `view_file` or `read_url_content`) to thoroughly read and analyze those documents.
- Automatically populate as much of `BA_Project_Checkpoint.md` as possible based purely on the provided documents.
- Sections to pre-fill if data is available:
  1. Identity & Baseline (Name, Domain, Problem)
  2. Stakeholders & Constraints
  3. High-Level Scope
  4. Methodological Tailoring

# 3. Iterative Q&A
- After analyzing the documents (or if starting from scratch), identify which mandatory fields in `BA_Project_Checkpoint.md` are still missing or require clarification.
- **CRITICAL EXCEPTION:** Do NOT ask the BA about their "Delivery Methodology" (e.g., Agile or Waterfall). This decision is formally made during the "Plan BA Approach" task, unless it was explicitly mandated in the provided Preparation documents.
- Ask the BA the missing questions **STRICTLY ONE AT A TIME**. Do NOT ask multiple questions in a single message.
- Wait for the BA to answer the single question before moving to the next one.
- As the BA answers, dynamically update `BA_Project_Checkpoint.md` in the background. Address them conversationally while doing so.

# 4. Knowledge Area Scaffolding
- When arriving at Section 4, ask the BA: "Based on what we've discussed, which of the 6 BABOK Knowledge Areas should we scaffold for this project? I can suggest the required ones or generate all of them." (Only ask this if it wasn't already determined from the documents).
- Once confirmed by the BA, check the boxes in `BA_Project_Checkpoint.md`.
- Based on the checked boxes, create the corresponding folders in the root directory:
  - `01_Planning_and_Monitoring`
  - `02_Elicitation_and_Collaboration`
  - `03_Requirements_Life_Cycle_Management`
  - `04_Strategy_Analysis`
  - `05_Requirements_Analysis_and_Design_Definition`
  - `06_Solution_Evaluation`

# 5. Finalization
- Inform the BA that the scaffold is complete and the `BA_Project_Checkpoint.md` is initialized.
- Remind the BA they can invoke specialized skills located in the `.agents/skills` folder to continue work within the generated Knowledge Areas.

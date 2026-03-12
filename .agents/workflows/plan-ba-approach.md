---
description: Guide the BA through selecting and documenting the Business Analysis Approach for the current project
---

# 1. Read Project Context
- Open and read `BA_Project_Checkpoint.md` from the project root.
- Extract: Project Name, Domain, Primary Business Problem, Stakeholder types, In/Out-of-Scope items.
- Do NOT ask the BA for information already captured there.

# 2. Approach Selection — One Question at a Time
Ask the BA the following questions **ONE AT A TIME**. Wait for each answer before proceeding.

- **Q1:** "How well are the project requirements understood right now — are they clearly defined upfront, or do you expect them to evolve significantly during delivery?"
- **Q2:** "How tolerant are your key stakeholders to change during the project — do they prefer a fixed plan with formal sign-off, or can they accommodate iterative delivery?"
- **Q3:** "Is there a regulatory, contractual or audit reason that requires formal documentation of decisions at each stage?"

# 3. Approach Determination
Based on answers, determine the appropriate approach:
- **Predictive** — Requirements clearly defined, low change tolerance, formal audit trail required
- **Adaptive** — Evolving requirements, high change tolerance, iterative delivery acceptable  
- **Hybrid** — Mixed signals across the three questions

# 4. Generate BA Approach Document
Create `01_Planning_and_Monitoring/BA_Approach_v1.md` containing:
- Selected Approach (Predictive / Adaptive / Hybrid) with rationale
- Key implications for how requirements will be elicited, approved, and changed
- Decision log referencing the BA's answers above

# 5. Update Checkpoint
- Update the `Selected Delivery Methodology` field in `BA_Project_Checkpoint.md` with the determined approach.
- Inform the BA: "Your BA Approach document has been created at `01_Planning_and_Monitoring/BA_Approach_v1.md`. You can refine this at any time as the project evolves."

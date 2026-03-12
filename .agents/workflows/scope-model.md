---
description: Generate a visual Mermaid context diagram showing the system boundary and all external actors interacting with it
---

# 1. Read Project Context
- Open and read `BA_Project_Checkpoint.md`.
- Extract: Project Name, In-Scope items, Out-of-Scope items, and the Stakeholder list.
- Also read `01_Planning_and_Monitoring/Stakeholder_Register_v1.md` if it exists.

# 2. Clarify the System Boundary — One Question at a Time
Ask the BA the following questions ONE AT A TIME:

- **Q1:** "What is the name of the system or solution we are defining scope for?" (e.g., "Dynamics 365 BC", "Customer Portal", "New Pricing Engine")
- **Q2:** "Which of the stakeholder groups directly interact with the system — meaning they send data into it or receive data from it?" (List candidates from Stakeholder Register)
- **Q3:** "Are there any external systems (not people) that the solution must connect to or exchange data with?" (e.g., legacy ERP, payment gateway, data warehouse)

# 3. Generate the Scope Model
Create `01_Planning_and_Monitoring/Scope_Model_v1.md` containing:

1. A **Mermaid context diagram** using `graph TD` format:
   - A central node representing the system/solution
   - Nodes for each stakeholder group that interacts with it (from Q2)
   - Nodes for each external system (from Q3)
   - Directed arrows showing the flow direction: who sends data and who receives it
   - A visual boundary (use subgraph) separating In-Scope from Out-of-Scope elements

2. A **Scope Boundary Table** below the diagram:
   | Element | Type | In/Out of Scope | Notes |
   |---|---|---|---|

# 4. Inform the BA
- "Your Scope Model is ready at `01_Planning_and_Monitoring/Scope_Model_v1.md`."
- "The Mermaid diagram will render automatically in Antigravity IDE. Refresh it as scope evolves."

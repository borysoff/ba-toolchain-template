# Business Analysis Toolchain Template
This is a self-extracting Business Analysis target environment designed directly for the Antigravity IDE. It accelerates project initialization by utilizing LLMs to flesh out standard BABOK artifacts contextually.

### Quickstart
1. **Initialize Project Checkpoint:** Run the Antigravity IDE slash command `/init-ba-project`.
2. **Q&A Flow:** The agent will ask you a series of contextual questions to establish project boundaries, constraints, stakeholders, and high-level scope. This takes around 5-10 minutes.
3. **Artifact Generation:** As the flow progresses, the agent will dynamically populate your `BA_Project_Checkpoint.md` file. It will then optionally scaffold and generate sub-documents across the 6 major knowledge areas based on your explicit needs.

### Directory Structure Structure
```text
/
├── .agents/workflows/   # Contains the /init-ba-project extraction script
├── 01_Planning_and_Monitoring/
├── 02_Elicitation_and_Collaboration/
├── 03_Requirements_Life_Cycle_Management/
├── 04_Strategy_Analysis/
├── 05_Requirements_Analysis_and_Design_Definition/
├── 06_Solution_Evaluation/
├── BA_Project_Checkpoint.md # Central contextual node
└── README.md
```

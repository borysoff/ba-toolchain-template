---
description: Build a structured Stakeholder Engagement Register from the project checkpoint data
---

# 1. Read Project Context
- Open and read `BA_Project_Checkpoint.md` from the project root.
- Extract the stakeholder list from Section 2.
- Also read `01_Planning_and_Monitoring/BA_Approach_v1.md` if it exists (engagement style depends on approach).

# 2. Enrich Each Stakeholder — One at a Time
For each stakeholder group identified in the Checkpoint, ask the following questions **ONE AT A TIME**, working through each stakeholder before moving to the next:

- **[Stakeholder Name] — Influence:** "How much decision-making power does [Stakeholder] have over project outcomes? (High / Medium / Low)"
- **[Stakeholder Name] — Interest:** "How directly does [Stakeholder] care about the project outcomes? (High / Medium / Low)"
- **[Stakeholder Name] — Current Attitude:** "What is [Stakeholder]'s current attitude toward this project? (Champion / Neutral / Sceptic / Unknown)"

# 3. Generate Stakeholder Register
Create `01_Planning_and_Monitoring/Stakeholder_Register_v1.md` with:
- A table containing: Stakeholder Group, Influence, Interest, Current Attitude, Engagement Strategy
- Auto-populate the **Engagement Strategy** column using standard rules:
  - High Influence + High Interest → "Manage Closely"
  - High Influence + Low Interest → "Keep Satisfied"
  - Low Influence + High Interest → "Keep Informed"
  - Low Influence + Low Interest → "Monitor"
- A notes section for sceptics flagging the risk of stakeholder resistance

# 4. Inform the BA
- "Your Stakeholder Register is ready at `01_Planning_and_Monitoring/Stakeholder_Register_v1.md`."
- Remind the BA: "Engagement strategies should be revisited at each major project milestone. Run `/stakeholder-register` again to refresh the register."

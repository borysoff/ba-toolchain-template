---
description: Build a structured Risk Register by guiding the BA through risk identification and scoring for the current project
---

# 1. Read Project Context
- Open and read `BA_Project_Checkpoint.md`.
- Extract: Project scope, stakeholder list, known constraints, and delivery methodology (if determined).
- Also read `01_Planning_and_Monitoring/BA_Approach_v1.md` if it exists.
- Do NOT ask for information already captured in these files.

# 2. Seed Risk Categories
Based on the project context, silently identify applicable risk categories from this list:
- **Stakeholder Risk** — Resistance, unavailability, conflicting priorities
- **Scope Risk** — Scope creep, unclear boundaries, late inclusions
- **Regulatory / Compliance Risk** — Domain-specific regulatory exposure
- **Technical Risk** — Legacy system constraints, integration complexity
- **Resource Risk** — BA availability, subject matter expert access
- **Governance Risk** — Approval delays, unclear decision authority

# 3. Risk Elicitation — One Risk Category at a Time
For each applicable category, ask the BA ONE question at a time:

- "For **[Category]**: Are there any specific risks you are already aware of in this area for this project?"
- Wait for the answer. Record any identified risks. Then move to the next category.
- If the BA says "none" for a category, log it as "No risks identified" and move on.

# 4. Score Each Risk
For each identified risk, ask the BA:
- "How likely is this risk to occur? (High / Medium / Low)"
- Wait for answer. Then ask:
- "If it occurs, how severe would the impact be? (High / Medium / Low)"
- Record both scores. Calculate a Risk Level:
  - High + High → 🔴 Critical
  - High + Medium or Medium + High → 🟠 High
  - Medium + Medium → 🟡 Medium
  - Low + anything or anything + Low → 🟢 Low

# 5. Generate Risk Register
Create `01_Planning_and_Monitoring/Risk_Register_v1.md` with:

```
| # | Risk Description | Category | Likelihood | Impact | Level | Mitigation Strategy |
```

- Auto-populate **Mitigation Strategy** with a sensible default based on category and level.
- Flag any 🔴 Critical risks with: "⚠️ Requires escalation to project governance log."

# 6. Inform the BA
- "Your Risk Register is ready at `01_Planning_and_Monitoring/Risk_Register_v1.md`."
- "Run `/risk-register` again at any project milestone to refresh and re-score risks."

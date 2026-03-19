---
description: Build a targeted elicitation session guide bounded by project context and stakeholder persona — prevents wasted interview time and stakeholder fatigue
---

# 1. Read Project Context
- Open and read `BA_Project_Checkpoint.md`.
- Scan `02_Elicitation_and_Collaboration/` for any existing context anchors (`ctx_*.md`) or prior session guides.
- If `01_Planning_and_Monitoring/Stakeholder_Register_v1.md` exists, read it to identify stakeholder profiles.
- Do NOT ask for information already captured in these files.

# 2. Identify the Session
Ask the BA ONE question at a time:

- **Q1:** "Which stakeholder or stakeholder group is this elicitation session for?"
- **Q2:** "What is the primary objective of this session — what specific decision, requirement, or area of uncertainty are we trying to resolve?"
- **Q3:** "Do you have a context anchor for this stakeholder already in `02_Elicitation_and_Collaboration/`? If yes, I will use it. If no, I will generate one now."

# 3. Create or Load the Context Anchor
- If a context anchor exists for this stakeholder, read it and proceed.
- If not, create `02_Elicitation_and_Collaboration/ctx_[stakeholder_name].md` using the `ctx_session_anchor.md` template, pre-filling what is known from the Checkpoint and Stakeholder Register.
- Inform the BA: "I have created a context anchor for [Stakeholder] at `02_Elicitation_and_Collaboration/ctx_[stakeholder_name].md`. Please review it and add any domain-specific details before the session."

# 4. Generate the Session Guide
Create `02_Elicitation_and_Collaboration/Session_Guide_[Stakeholder]_v1.md` containing:

### Session Header
- Stakeholder, Date (TBD), Objective, Facilitator

### Pre-Session Document Analysis
- List the specific documents the BA must read BEFORE the session (from context anchor and `00_Preparation/`)
- One-line note on WHY each document matters for this specific stakeholder

### Opening Question
- One single opening question designed to let the stakeholder speak freely before structured probing begins

### Targeted Probe Questions (max 8)
- Each question must target a specific known gap, risk, or conflict from the project context
- Format: Question → What we are trying to discover → Acceptable answer signals

### Conflict Watchlist
- List 2–4 specific friction points to watch for based on what is already known from the Checkpoint and other stakeholder positions

### Closing
- Standard wrap: "Is there anything important you feel we have not covered?"

# 5. Inform the BA
- "Your session guide is ready at `02_Elicitation_and_Collaboration/Session_Guide_[Stakeholder]_v1.md`."
- "After the session, drop the raw transcript into `02_Elicitation_and_Collaboration/` and run `/conflict-register` to synthesize findings."

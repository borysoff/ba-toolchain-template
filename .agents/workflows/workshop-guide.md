---
description: Build a structured workshop or focus group agenda for a multi-stakeholder elicitation session, bounded by known conflicts and decision goals
---

# 1. Read Project Context
- Read `BA_Project_Checkpoint.md` — extract Stakeholders, Scope, and Methodology.
- Read `01_Planning_and_Monitoring/Stakeholder_Register_v1.md` if it exists.
- Read `02_Elicitation_and_Collaboration/Conflict_Register_v1.md` if it exists — conflicts to resolve in the workshop.
- Read any relevant `ctx_*.md` files for the participating stakeholders.

# 2. Define the Session — One Question at a Time
- **Q1:** "Who will be attending this workshop?" (list stakeholder groups)
- **Q2:** "What is the primary decision or outcome this workshop must produce?"
- **Q3:** "Is this a requirements elicitation workshop, a conflict resolution session, a review/sign-off workshop, or something else?"
- **Q4:** "How much time is allocated for the session?" (e.g., 2 hours, half day)

# 3. Generate Workshop Agenda
Create `02_Elicitation_and_Collaboration/Workshop_Guide_[Topic]_v1.md` containing:

### Session Header
| Field | Value |
|---|---|
| Topic | [From Q2] |
| Type | [Elicitation / Conflict Resolution / Review] |
| Attendees | [From Q1] |
| Duration | [From Q4] |
| Facilitator | [BA — to fill in] |
| Target Output | [Document or decision to be produced] |

### Pre-Workshop Checklist
- Documents to distribute in advance (from context anchors and `00_Preparation/`)
- Known conflicts to resolve (from Conflict Register — 🔴 Blocking items prioritised)
- Open questions to force a decision on (from `ctx_*.md` files)

### Agenda (Timed)
Auto-generate a timed agenda based on session type and duration:
- **Opening** (5 min) — Objectives, ground rules, desired output
- **Context Setting** (10 min) — BA presents known state and open items
- **Structured Elicitation Blocks** — One block per major topic/conflict, timebox proportional to total duration
- **Decision Capture** (10 min) — Explicitly call each open decision, record Yes/No/Deferred
- **Action Items** (5 min) — Who does what by when
- **Close**

### Facilitation Notes
- List 2–3 specific facilitation risks for this group (from Stakeholder Register attitudes)
- Suggested intervention if the session gets stuck on a blocking conflict

### Post-Workshop Actions
- Drop raw notes or transcript into `02_Elicitation_and_Collaboration/` as `transcript_[Topic]_[Date].md`
- Run `/conflict-register` to synthesize outputs
- Update `Elicitation_Log.md`

# 4. Inform the BA
"Your Workshop Guide is ready at `02_Elicitation_and_Collaboration/Workshop_Guide_[Topic]_v1.md`. After the session, drop the raw notes into `02_Elicitation_and_Collaboration/` and run `/conflict-register`."

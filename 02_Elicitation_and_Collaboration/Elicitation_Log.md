# Elicitation Log
**Project:** [From BA_Project_Checkpoint.md]
**Last Updated:** [Date]

> **Purpose:** The official record of all elicitation activity. Each row represents one elicitation session. Raw transcripts should be stored in this folder as `transcript_[Stakeholder]_[Date].md`. This log is the reference used by `/conflict-register` and `/verify-elicitation`.
>
> **How to use with the agent:** Say "Log a new session: [stakeholder], [date], [method], [topic]" and the agent will append a row.

---

## Session Log

| # | Date | Stakeholder(s) | Method | Session Topic / Objective | Transcript File | Status | Key Outputs |
|---|---|---|---|---|---|---|---|
| EL-001 | [Date] | [Stakeholder] | [Interview / Workshop / Focus Group / Document Review] | [What was the objective?] | [transcript_file.md] | ⬜ Draft / ✅ Confirmed | [e.g., 3 requirements, 1 conflict] |

---

## Status Reference
| Status | Meaning |
|---|---|
| ⬜ Draft | Session held, transcript not yet verified |
| 🔄 In Review | `/conflict-register` or `/verify-elicitation` run — awaiting BA sign-off |
| ✅ Confirmed | BA has reviewed and confirmed the session outputs are accurate |
| ❌ Contested | A stakeholder has disputed the session record — resolution required |

---

## Elicitation Coverage Tracker
*Track which in-scope areas have been covered by at least one confirmed session.*

| In-Scope Area | Covered? | Session(s) |
|---|---|---|
| [From BA_Project_Checkpoint.md — In-Scope items] | ⬜ / ✅ | [EL-xxx] |

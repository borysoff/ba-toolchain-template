---
description: Synthesize one or more elicitation transcripts to produce a structured Conflict Register and Wants vs Needs classification
---

# 1. Locate Source Material
- Scan `02_Elicitation_and_Collaboration/` for raw transcript files (any `.md` files prefixed with `transcript_` or `session_`).
- Also read any relevant context anchors (`ctx_*.md`) for the stakeholders whose transcripts are being processed.
- Read `BA_Project_Checkpoint.md` — specifically the In-Scope/Out-of-Scope section and the primary business problem.
- If a Project Charter or Business Case exists in `00_Preparation/`, read it — it is the authoritative reference for classifying Wants vs. Needs.

# 2. Ask for Scope — One Question at a Time
- **Q1:** "Which transcript file(s) should I synthesize? List the filenames or say 'all' to process all transcripts in `02_Elicitation_and_Collaboration/`."
- Wait for answer, then proceed.

# 3. Perform Multi-Source Synthesis
For each transcript provided:
- Extract every **stated requirement, preference, or constraint** raised by each stakeholder.
- Classify each item as:
  - ✅ **Underlying Need** — Directly serves the core business problem in the Checkpoint / Charter
  - ⚠️ **Stated Want** — Expressed preference not directly tied to the core business problem
  - 🔴 **Potential Conflict** — Contradicts another stakeholder's position or the project Charter

# 4. Generate Conflict Register
Create `02_Elicitation_and_Collaboration/Conflict_Register_v1.md` containing:

### Section 1: Wants vs Needs Classification Table
| # | Stakeholder | Statement | Classification | Basis for Classification |
|---|---|---|---|---|

### Section 2: Conflict Log
| # | Conflicting Parties | Point of Conflict | Stakeholder A Position | Stakeholder B Position | Severity | Resolution Status |
|---|---|---|---|---|---|---|

Severity scale: 🔴 Blocking (must resolve before design) / 🟠 High / 🟡 Medium / 🟢 Low

### Section 3: Open Items Requiring BA Decision
- List any items where classification was ambiguous and a human judgment call is required.

# 5. Inform the BA
- "Your Conflict Register is ready at `02_Elicitation_and_Collaboration/Conflict_Register_v1.md`."
- "Blocking conflicts (🔴) must be resolved before requirements can be baselined. Run `/verify-elicitation` to check coverage."

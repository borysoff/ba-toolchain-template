---
description: Verify elicitation completeness — checks coverage of in-scope areas and flags gaps before requirements can be baselined
---

# 1. Read Source Material
- Read `BA_Project_Checkpoint.md` — extract In-Scope items and Stakeholder list.
- Read `02_Elicitation_and_Collaboration/Elicitation_Log.md` — identify which sessions are Confirmed vs Draft/Contested.
- Read `02_Elicitation_and_Collaboration/Conflict_Register_v1.md` if it exists — check for unresolved Blocking conflicts.
- Read any context anchors (`ctx_*.md`) in `02_Elicitation_and_Collaboration/` to extract Open Questions.

# 2. Run Coverage Check
For each In-Scope item in the Checkpoint:
- Check whether at least one ✅ Confirmed elicitation session covers it.
- Flag any item with no confirmed coverage as a **Gap**.

For each Stakeholder in the Checkpoint:
- Check whether they appear in at least one Confirmed session.
- Flag any stakeholder with no confirmed session as a **Coverage Risk**.

# 3. Run Conflict Resolution Check
- Identify any 🔴 Blocking conflicts in the Conflict Register that are still marked "Unresolved".
- These must be resolved before requirements can be baselined.

# 4. Run Open Questions Check
- Scan all context anchors for items listed in "Open Questions Assigned to This Stakeholder".
- Flag any that have not been answered in a Confirmed session or the Conflict Register.

# 5. Generate Verification Report
Create `02_Elicitation_and_Collaboration/Elicitation_Verification_Report_v1.md` containing:

### Coverage Scorecard
| In-Scope Area | Covered? | Sessions | Gap? |
|---|---|---|---|

### Stakeholder Coverage
| Stakeholder | Session Count | Last Session | Gap? |
|---|---|---|---|

### Blocking Items
| Type | Description | Source | Action Required |
|---|---|---|---|
| [Blocking Conflict / Open Question / Unconfirmed Session] | | | |

### Verdict
- ✅ **Ready to baseline** — if all In-Scope items covered, no blocking conflicts, no unanswered open questions
- ⚠️ **Conditional** — minor gaps exist but do not block design (list them)
- ❌ **Not ready** — blocking items must be resolved first (list them)

# 6. Inform the BA
- "Your Elicitation Verification Report is at `02_Elicitation_and_Collaboration/Elicitation_Verification_Report_v1.md`."
- If verdict is ✅: "You are cleared to move to KA3: Requirements Life Cycle Management."
- If verdict is ❌: "The following items must be resolved before baselining requirements: [list blocking items]."

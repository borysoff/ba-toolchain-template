---
description: Run a structured KPI retrospective at a project stage gate to assess BA performance and extract lessons learned
---

# 1. Establish Review Scope
Ask the BA ONE question at a time:

- **Q1:** "Which stage or milestone are we reviewing?" (e.g., Stage 1, Sprint 3, Planning Phase)
- **Q2:** "What were the agreed performance targets for this stage? (e.g., deliver X artefacts, complete elicitation by date Y, zero compliance gaps)"

If targets were not formally defined, suggest using these defaults:
- Speed: Delivery on or ahead of schedule
- Quality: No artefacts rejected at review
- Completeness: All required artefacts produced

# 2. Evidence Scan
- Scan the relevant KA folder (e.g., `01_Planning_and_Monitoring/`) for all artefacts produced during the stage.
- List each artefact found with its creation date and estimated completeness.

# 3. Generate Performance Assessment
Create `01_Planning_and_Monitoring/BA_Performance_Assessment_[StageName].md` containing:

### KPI Scorecard
| KPI | Target | Evidence | Rating | Score |
|---|---|---|---|---|
| Speed | [from Q2] | [artefact list] | ✅/⚠️/❌ | /5 |
| Quality | [from Q2] | [review status] | ✅/⚠️/❌ | /5 |
| Completeness | [from Q2] | [artefact count] | ✅/⚠️/❌ | /5 |

### Root Cause Analysis
- For any KPI rated ⚠️ or ❌, document a brief root cause and corrective action.

### Lessons Learned
- Extract at least 3 lessons learned from the stage evidence.

# 4. Inform the BA
- "Your Performance Assessment is at `01_Planning_and_Monitoring/BA_Performance_Assessment_[StageName].md`."
- Ask: "Would you like to escalate any findings to the project governance log?"

# Context Anchor: [Stakeholder Name / Session Topic]
**Purpose:** This file bounds the agent's reasoning to a specific stakeholder context. The agent reads this file before conducting any elicitation-related task for this stakeholder. Do not use general knowledge not contained here.

---

## 1. Stakeholder Profile
<!-- Who are we talking to? What drives them? What do they fear? -->

**Name / Role:** [e.g., CFO, Head of IT, Lead Consultant]
**Primary Mandate:** [What is this person responsible for delivering in the organization?]
**Known Pain Points:** 
- [e.g., Month-end close takes too long]
- [e.g., Audit findings from last FY]

**Known Position on This Project:**
- [Champion / Sceptic / Neutral / Unknown]
- [Any known stance on key scope items?]

---

## 2. Domain Constraints Relevant to This Stakeholder
<!-- What regulatory, financial, or technical rules govern what this stakeholder can and cannot agree to? -->
<!-- Only include rules confirmed by authoritative documents — no assumptions. -->

- [e.g., "CFO approval is required for any change to revenue recognition logic per Company Policy 4.2"]
- [e.g., "IFRS 15 §B18 allows hours-based PoC measurement if data quality is demonstrably high"]

**Source Documents:** [List documents this was extracted from]

---

## 3. Known Conflicts or Tensions
<!-- What do we already know that this stakeholder disagrees with — from other stakeholders, documents, or prior sessions? -->

| Conflict | This Stakeholder's Position | Conflicting Party | Notes |
|---|---|---|---|
| [e.g., PoC measurement method] | [e.g., Cost-based] | [e.g., PMO Director] | [Source: Session 1 transcript] |

---

## 4. Open Questions Assigned to This Stakeholder
<!-- What specific unknowns must this person resolve before requirements can be baselined? -->

1. [Question / decision gap]
2. [Question / decision gap]

---

## 5. Out-of-Bounds Topics
<!-- Topics the agent must NOT raise with this stakeholder — political, premature, or legally sensitive. -->

- [e.g., Do not raise FR-007 until legal review is complete]
- [e.g., Do not discuss budget overrun — escalation is with the Sponsor only]

---

> **Agent Instruction:** Before generating any session guide or synthesis for this stakeholder, read this file in full. Do not make claims about this stakeholder's position that are not documented here.

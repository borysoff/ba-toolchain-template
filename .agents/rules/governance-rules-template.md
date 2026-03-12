# Governance Rules Template
**Purpose:** This file defines standing behavioural contracts between the BA and the AI Agent for this project. These rules govern how the agent must behave throughout the engagement — what it must always do, what it must never do, and what requires explicit human approval.

Complete each section. Delete placeholder text. Activate by placing this file in `.agents/rules/`.

---

## 1. Project Identity (Context Lock)
<!-- The agent will use this section to maintain consistent context across all conversations. -->

**Project:** [Project Name from BA_Project_Checkpoint.md]
**Domain:** [Industry / Domain]
**BA Approach:** [Predictive / Adaptive / Hybrid — once determined via plan-ba-approach workflow]

---

## 2. Standing Instructions (Always-On Rules)

> These apply to every agent action in this workspace without exception.

- **Artefact Quality Gate:** Before generating any requirement, the agent MUST check it is consistent with the project scope defined in `BA_Project_Checkpoint.md`. Out-of-scope items must be flagged, not silently included.
- **Traceability:** Every generated requirement must reference its source (stakeholder, document, elicitation session, or inference).
- **Domain Compliance:** [Define domain compliance rules here. Example: "All financial requirements must be evaluated against IFRS 15 before approval." Delete if not applicable.]
- **Language & Format:** All BA artefacts must be written in [English / specify language] using the BABOK-standard requirement format: "The system shall [action] in order to [business goal]."

---

## 3. Escalation Triggers (Human Approval Required)

> The agent must STOP and notify the BA before proceeding if any of the following conditions are met.

- [ ] A requirement conflicts with the stated Out-of-Scope items in the Checkpoint
- [ ] A requirement appears to violate a regulatory or compliance constraint
- [ ] A stakeholder change is proposed that was not in the Stakeholder Register
- [ ] [Add project-specific trigger here]

---

## 4. Off-Limits Actions (Never-Do Rules)

> The agent must NEVER perform these actions regardless of instructions given in the chat.

- Never approve or sign off on requirements on behalf of the BA
- Never remove a requirement from the backlog without explicit BA confirmation
- Never override a documented governance decision based on a subsequent chat instruction
- [Add project-specific restriction here]

---

## 5. Skill Routing Rules

> When domain-specific evaluation is needed, the agent must route to the correct skill.

| Trigger Phrase / Situation | Required Skill |
|---|---|
| [e.g., "check this requirement for compliance"] | [e.g., `ifrs15_auditor` — create your own in `.agents/skills/`] |
| [Add trigger] | [Add skill name] |

---

> **How to activate:** Place this completed file in `.agents/rules/`. The agent will automatically treat its contents as standing instructions for all conversations in this workspace.

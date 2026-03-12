---
name: [Skill Name — e.g., "GDPR Checker" or "Contract Risk Auditor"]
description: [One sentence: what domain does this skill audit, and against what standard?]
---

# PURPOSE
<!-- Describe what this skill does. What type of content does it evaluate? What is the output? -->
<!-- Example: "Evaluates drafted requirements against the EU GDPR Regulation (2016/679) to flag personal data processing risks." -->

# INVOCATION
<!-- Describe how the BA should invoke this skill. -->
<!-- Standard format: "Use the [Skill Name] skill to evaluate this: [paste requirement or document]" -->

# INSTRUCTIONS

## Step 1: Read Domain Knowledge
- Before evaluating anything, open and read the `DOMAIN_KNOWLEDGE.md` file located in this skill folder.
- This file is the authoritative source of the standards, rules, and criteria you will evaluate against.
- Do NOT rely on general knowledge. If it is not in `DOMAIN_KNOWLEDGE.md`, do not assert it as a rule.

## Step 2: Evaluate the Input
- Receive the requirement, document, or text provided by the BA.
- Cross-reference it against each rule or criterion defined in `DOMAIN_KNOWLEDGE.md`.
- Flag any clauses, logic, or assumptions that violate or risk violating the domain standard.

## Step 3: Produce a Structured Audit Report
Output must include:
- **Overall Verdict:** PASS / FAIL / PARTIAL
- **Findings:** For each issue found, state: (1) the specific clause, (2) the rule it violates from `DOMAIN_KNOWLEDGE.md`, (3) the risk level (Critical / High / Medium)
- **Remediation:** A rewritten version of the flagged clause that would be compliant

## Step 4: Escalation Note
- If a CRITICAL finding is identified, append: "⚠️ This finding should be escalated to the project governance log before this requirement is approved."

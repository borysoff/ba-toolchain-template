# Domain Knowledge
**Purpose:** This file is the authoritative knowledge source for the `[Skill Name]` skill. The agent reads this file before evaluating any input. All rules, frameworks, and standards referenced in `SKILL.md` must be defined here.

---

## Standard / Framework Reference
<!-- Identify the authoritative source this knowledge is based on. -->
<!-- Example: "IFRS 15 — Revenue from Contracts with Customers (IASB, 2014)" -->
<!-- Example: "EU GDPR Regulation (2016/679)" -->

**Source:** [Name of standard, regulation, or framework]
**Version / Effective Date:** [e.g., "Effective January 2018"]
**Jurisdiction:** [e.g., "All EU member states" / "Global" / "UK only"]

---

## Core Rules / Criteria
<!-- Define the specific rules the agent must evaluate requirements against. -->
<!-- Be explicit. Vague rules produce vague audit results. -->
<!-- Example format: -->

### Rule 1: [Rule Title]
- **Statement:** [Full rule as it should be applied]
- **Pass Condition:** [What a compliant requirement looks like]
- **Fail Condition:** [What a non-compliant requirement looks like]
- **Example of Violation:** [Optional but highly recommended]

### Rule 2: [Rule Title]
- **Statement:**
- **Pass Condition:**
- **Fail Condition:**

<!-- Add as many rules as needed. Each should map directly to a real clause in your source standard. -->

---

## Key Distinctions & Edge Cases
<!-- Document nuances that would cause hallucination if left undefined. -->
<!-- Example: "Invoicing a client (billing) is NOT the same as recognizing revenue in the ledger." -->

- [Distinction 1]
- [Distinction 2]

---

## Glossary
<!-- Define domain-specific terms to prevent misinterpretation. -->

| Term | Definition |
|---|---|
| [Term] | [Definition] |

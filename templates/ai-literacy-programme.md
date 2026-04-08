# AI Literacy Programme Template (Article 4)

**Version:** 2.1.0
**Regulatory Basis:** EU AI Act Article 4

Article 4 of the EU AI Act imposes a **horizontal obligation** on all providers and deployers of AI systems — regardless of risk classification — to ensure that their staff and any other persons dealing with the operation and use of AI systems on their behalf have a **sufficient level of AI literacy**. This obligation has been in force since **2 February 2025**.

This template provides a practical framework for implementing an AI literacy programme that satisfies Article 4 and can be evidenced to regulators.

---

## 1. What Is "AI Literacy" Under Article 4?

AI literacy is defined in Article 3(56) as: *"skills, knowledge and understanding that allow providers, deployers and affected persons, taking into account their respective rights and obligations in the context of this Regulation, to make an informed deployment of AI systems"*.

**Key points:**
*   It applies to **all** AI systems, not just high-risk ones.
*   The level of literacy required must be **proportionate** to the context, the technical knowledge of the person, and the intended use of the AI system.
*   It is an **ongoing obligation**, not a one-off training event.

---

## 2. Needs Assessment Matrix

Before designing the programme, map the different roles in your organisation and the AI literacy level each requires.

| Role Category | Examples | Literacy Level Required | Focus Areas |
| :--- | :--- | :--- | :--- |
| **Executive Leadership** | CEO, CFO, Board Members | Foundational | Strategic AI risks, regulatory exposure (fines, liability), governance responsibilities, fiduciary duty in AI oversight. |
| **Legal & Compliance** | DPO, Legal Counsel, Compliance Officers | Intermediate | EU AI Act obligations (classification, conformity, FRIA), GDPR Art. 22, liability framework, incident notification duties. |
| **Technical Staff** | Data Scientists, ML Engineers, DevOps | Advanced | Model development lifecycle, bias detection and mitigation, security (prompt injection, model inversion), logging requirements (Art. 12), technical documentation (Annex IV). |
| **Procurement** | Vendor Managers, IT Procurement | Intermediate | [Vendor audit methodology](vendor-audit-checklist.md), DPA requirements, GPAI provider obligations, assessing CE marking and conformity documentation. |
| **Operational Users** | HR Managers, Customer Service Leads, Marketing | Foundational-Intermediate | Understanding AI outputs vs. decisions, [acceptable use policy](acceptable-use-policy.md), human oversight responsibilities (Art. 14), output verification (hallucination risks). |
| **All Employees** | Company-wide | Foundational | [Acceptable AI use policy](acceptable-use-policy.md), [Shadow AI risks](shadow-ai-risk-calculator.md), [IP protection in prompts](prompt-ip-guidelines.md), data classification rules, reporting suspected AI incidents. |

---

## 3. Core Curriculum Modules

### Module 1: AI Fundamentals (All Employees — 45 min)
*   What is AI? How do LLMs and generative AI work (non-technical overview).
*   The difference between deterministic software and probabilistic AI output.
*   Why AI "hallucinates" — understanding confidence vs. accuracy.
*   Your organisation's [Acceptable AI Use Policy](acceptable-use-policy.md).

### Module 2: Regulatory Landscape (Legal, Compliance, Procurement — 90 min)
*   EU AI Act structure: risk classification (Prohibited → Minimal), key obligations by role (Provider, Deployer, Distributor).
*   GDPR intersection: Article 22 (automated decision-making), Article 35 (DPIA), Article 9 (special categories).
*   EU AI Act enforcement timeline (see [Timeline](../assets/eu-ai-act-timeline.mmd)): what's in force now, what's coming in November 2026 (transparency) and December 2027 (high-risk).
*   Penalty structure: €35M/7% for prohibited practices, €15M/3% for high-risk violations, €7.5M/1% for incorrect information.

### Module 3: Responsible AI for Technical Teams (Data Science, Engineering — 120 min)
*   [Algorithmic bias audit methodology](../guides/algorithmic-bias-audit-methodology.md): fairness metrics, impossibility theorems, practical audit steps.
*   Data governance under Article 10: training data provenance, representativeness, bias testing.
*   Security threats: prompt injection, data poisoning, model inversion, adversarial attacks.
*   Logging and documentation requirements: Article 12 (automatic recording), Annex IV (technical documentation).

### Module 4: Human Oversight in Practice (Operational Users — 60 min)
*   What "meaningful human oversight" means under Article 14 — not rubber-stamping.
*   How to critically evaluate AI outputs: when to override, when to escalate.
*   Documenting human review decisions for audit trails.
*   [Incident response](ai-incident-response-playbook.md): when and how to report AI anomalies.

---

## 4. Delivery & Assessment

| Element | Requirement |
| :--- | :--- |
| **Delivery Format** | Blend of e-learning modules and in-person workshops (recommended). |
| **Frequency** | Initial training within 30 days of hire/role change. Annual refresher for all staff. Ad-hoc updates when significant regulatory changes occur. |
| **Assessment** | Short quiz at the end of each module (minimum 80% pass rate). Practical scenario-based exercise for Modules 3 and 4. |
| **Record-Keeping** | Maintain a training register documenting: employee name, role, module(s) completed, date, assessment score. Retain for the duration of employment + 3 years. |
| **Language** | Training must be provided in a language the employee understands. |

---

## 5. Evidencing Compliance to Regulators

If a national Market Surveillance Authority (MSA) or Data Protection Authority (DPA) requests evidence of AI literacy compliance:

*   [ ] Produce the AI Literacy Programme document (this template, customised).
*   [ ] Provide the training register with completion rates.
*   [ ] Demonstrate that the programme is proportionate to the roles and AI systems in use.
*   [ ] Show evidence of regular updates (e.g., the programme was updated after the Digital Omnibus trilogue finalisation).

---
*This template is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 1 — Assess & Contain**, **Step 1.4: Implement AI Literacy**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

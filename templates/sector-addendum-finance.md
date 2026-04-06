# AI Compliance Framework: Financial Services Addendum

**Version:** 1.0
**Regulatory Context:** April 2026

This addendum extends the core AI Compliance Framework for organizations operating in the Financial Services sector (banks, insurers, asset managers, fintechs). It maps the core templates to sector-specific regulations including DORA, MiFID II, and specific EU AI Act Annex III classifications.

---

## 1. EU AI Act Risk Classification for Finance

Financial services deploy AI in high-stakes environments. The EU AI Act (Regulation 2024/1689) explicitly classifies certain financial use cases as **High-Risk (Annex III)**, triggering stringent compliance obligations.

| AI Use Case | EU AI Act Classification | Key Regulatory Drivers |
| :--- | :--- | :--- |
| **Credit Scoring & Loan Approval** | 🔴 **High-Risk** (Annex III, 5b) | Must comply with full Title III obligations (risk management, data governance, technical documentation, human oversight). *Exception: SMEs providing interest-free deferred payment.* |
| **Life & Health Insurance Pricing** | 🔴 **High-Risk** (Annex III, 5c) | AI used for risk assessment and pricing in life and health insurance requires full conformity assessment. |
| **Algorithmic Trading** | 🟡 **Limited/Minimal Risk*** | *Not explicitly high-risk under AI Act, but heavily regulated by MiFID II (Article 17) requiring algorithmic testing and circuit breakers. |
| **Fraud Detection / AML** | 🟡 **Limited/Minimal Risk*** | *Unless it leads to decisions significantly impacting access to essential services. Requires strong GDPR Article 22 safeguards. |
| **Customer Service Chatbots** | 🟢 **Minimal Risk** | Subject to Article 50 transparency obligations (users must know they are interacting with an AI). |

---

## 2. DORA (Digital Operational Resilience Act) Integration

As of January 2025, DORA (Regulation (EU) 2022/2554) applies to all financial entities. AI systems are classified as ICT systems under DORA.

**How to adapt the core framework for DORA:**
*   **Vendor Audit Checklist:** When using the `vendor-audit-checklist.md` for an AI provider, you must also assess them as an "ICT Third-Party Service Provider" under DORA Chapter V. This requires specific contractual clauses regarding access, inspection, and audit rights.
*   **Incident Reporting:** AI model drift or hallucinations that cause operational disruption must be classified and reported under DORA's ICT-related incident reporting framework (Articles 17-20).
*   **Resilience Testing:** AI systems must be included in the annual digital operational resilience testing program (Article 24).

---

## 3. GDPR Article 22 & Credit Scoring

The intersection of AI credit scoring and GDPR Article 22 (Automated individual decision-making) is the most heavily scrutinized area by Data Protection Authorities (DPAs).

**Mandatory Safeguards:**
If you use AI for credit scoring (even if it's just a component of the decision), you must implement the following safeguards to comply with GDPR Art. 22(3):
1.  **Right to Human Intervention:** The applicant must have a clear, accessible way to request a human review of the AI-generated score.
2.  **Right to Express Point of View:** The applicant must be able to provide additional context that the AI may have missed.
3.  **Right to Contest:** A formal process to challenge the decision.

*Action Item:* Ensure your `acceptable-use-policy.md` explicitly prohibits the deployment of fully automated credit scoring systems without these three technical and operational safeguards in place.

---

## 4. MiFID II & Robo-Advisors

For asset managers and wealthtechs using AI for investment advice (Robo-advisors):

*   **Suitability (Article 25):** The AI algorithm must be demonstrably capable of assessing the client's knowledge, financial situation, and risk tolerance accurately. The logic cannot be a "black box."
*   **Explainability:** You must be able to explain to a regulator *why* the AI recommended a specific portfolio allocation for a specific client on a specific date.

---

## 5. Immediate Action Plan (April 2026)

1.  **Inventory High-Risk Systems:** Immediately identify any AI systems used for credit scoring or life/health insurance pricing. These are Annex III High-Risk systems.
2.  **Conduct AI-Specific DPIAs:** Use the `dpia-ai-template.md` for all credit scoring and fraud detection models. Standard IT DPIAs are insufficient.
3.  **Update DORA Register:** Ensure all third-party AI APIs (e.g., OpenAI, Anthropic) used in production are logged in your DORA Register of Information.

---
*This addendum is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 2 — Audit & Procure**, **Step 2.2: Map Sector-Specific Obligations**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

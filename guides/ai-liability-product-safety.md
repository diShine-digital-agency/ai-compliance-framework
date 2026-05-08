# AI Liability & Product Safety Guide for the European Market

**Version:** 2.4.0
**Regulatory Context:** May 2026

The EU AI Act defines the *rules* for AI systems, but it does not create a private right of action for individuals harmed by AI. Until late 2025, that role was expected to fall to two complementary instruments: the **AI Liability Directive** (proposed) and the **revised Product Liability Directive** (Directive 2024/2853). The European Commission **withdrew the AI Liability Directive proposal in 2025** (notice published in the Official Journal on 6 October 2025). The EU now operates a **two-pillar liability framework**: the AI Act sets rules and the revised PLD provides strict liability for defective AI products. Fault-based AI claims fall under **national tort law** in each Member State.

This guide explains the liability exposure for enterprises deploying or providing AI systems in the European market.

---

## 1. The Two Pillars of EU AI Regulation (Post-AILD Withdrawal)

| Pillar | Instrument | Function | Status (May 2026) |
| :--- | :--- | :--- | :--- |
| **Rules** | EU AI Act (Regulation 2024/1689) | Sets obligations for providers, deployers, importers, distributors. Defines prohibited practices and high-risk requirements. | In force. Phased application: prohibited practices (Feb 2025), GPAI (Aug 2025), Article 50 transparency (2 December 2026 under Omnibus, provisional 7 May 2026), high-risk (2 December 2027 under Omnibus). |
| **Strict Liability** | Revised Product Liability Directive (Directive 2024/2853) | Extends product liability to software and AI systems. Enables claims for defective AI products without proving fault. | Adopted December 2024. Member States must transpose by **9 December 2026**. |

**Withdrawn:** The AI Liability Directive proposal (COM/2022/496) was formally withdrawn by the Commission on 16 July 2025; notice of withdrawal published in the OJ on **6 October 2025**. There is currently no AI-specific fault-based liability instrument at EU level.

---

## 2. The Revised Product Liability Directive (2024/2853)

### What Changed?
The original Product Liability Directive (85/374/EEC) was designed for physical products. The revised directive explicitly includes:
*   **Software** (including AI systems) as a "product."
*   **AI-enabled products** (e.g., a robot guided by AI, a medical device with AI diagnostics).
*   **Digital services** that are integrated into or interconnected with a product (e.g., OTA updates that alter product behaviour).

### Key Provisions for AI

| Provision | Impact on AI Providers/Deployers |
| :--- | :--- |
| **Software = Product** | Standalone AI software is now a "product" under the directive. If it is defective and causes damage, the provider is strictly liable (no need to prove fault). |
| **Defect Definition** | An AI system is "defective" if it does not provide the safety a person is entitled to expect, considering: (a) its presentation and marketing; (b) the use to which it could reasonably be put; (c) the effect on the product of **any ability to continue to learn** after deployment. |
| **Learning Systems** | The directive explicitly addresses AI systems that learn and evolve after deployment. If a post-deployment update (including autonomous learning) introduces a defect, the provider may be liable. |
| **Disclosure of Evidence** | Courts can order a defendant (AI provider) to disclose relevant evidence, including technical documentation and source code, to help the claimant prove their case. Safeguards exist for trade secrets. |
| **Burden of Proof (Lightened)** | If a claimant cannot access sufficient evidence to prove causation (e.g., because the AI is a "black box"), the court can **presume** that the defect caused the damage. |
| **Damage Types** | Covers death, personal injury, damage to property, and — newly — **destruction or corruption of data** not used exclusively for professional purposes. Psychological harm is covered if medically recognised. |

### Transposition Deadline
Member States must transpose the revised directive into national law by **9 December 2026**. Until then, the original 85/374/EEC directive applies, but enterprises should already adapt their risk management.

---

## 3. The AI Liability Directive — Withdrawn

### Status
The AI Liability Directive (COM/2022/496) was a proposed directive intended to complement the revised Product Liability Directive by covering **fault-based** (negligence) claims. The Commission announced the intention to withdraw in the February 2025 work programme citing "no foreseeable agreement", formally decided to withdraw on **16 July 2025**, and the notice of withdrawal was published in the OJ on **6 October 2025**.

### Why Withdrawn
- Stakeholder disagreement after more than two years of stalled negotiations.
- The regulatory simplification agenda underlying the Digital Omnibus package.
- Assessment that the revised PLD plus AI Act compliance evidence already address most of the original purpose.

### Practical Effect
- There is currently **no AI-specific fault-based liability instrument at EU level**.
- Fault-based AI claims continue to be governed by **national tort law** in each Member State, with substantial variation in:
  - Standard of care
  - Burden of proof rules
  - Disclosure of evidence mechanisms
  - Statute of limitations
- The presumption-of-causality and disclosure-of-evidence mechanisms that the AILD would have harmonised across the EU are **not available**.
- The Commission has signalled it may revisit the topic but has no active proposal as of May 2026. Practitioners should monitor the Commission's annual work programme.

---

## 4. Practical Implications for Enterprises

### For Providers (AI System Developers)
*   **Compliance = Liability Shield:** Strict compliance with the EU AI Act (especially risk management under Article 9, technical documentation under Annex IV, and post-market monitoring under Article 72) directly reduces your exposure under the revised PLD's defectiveness presumption and under national tort regimes. See the [Conformity Assessment Guide](../templates/conformity-assessment-guide.md).
*   **Post-Deployment Monitoring:** The revised Product Liability Directive makes you potentially liable for defects introduced by post-deployment learning. Implement robust monitoring and rollback capabilities.
*   **Insurance:** Consider AI-specific product liability insurance. Traditional technology E&O policies may not cover AI system defects.
*   **Track National Tort Developments:** With the AILD withdrawn, exposure now varies significantly across Member States. Map the rules of each market where you operate.

### For Deployers (AI System Users)
*   **Vendor Contracts:** When using the [Vendor Audit Checklist](../templates/vendor-audit-checklist.md), ensure contracts include:
    *   Clear liability allocation and indemnification for AI system defects.
    *   Right to access logs and technical documentation in the event of a claim.
    *   Vendor obligation to cooperate in court-ordered evidence disclosure.
    *   Choice of law and forum clauses with attention to which Member State's tort regime will govern fault-based claims.
*   **Human Oversight Documentation:** Document every instance of human oversight for high-risk AI systems. Under most national tort regimes, "rubber-stamped" AI decisions without genuine review are likely to be treated as breaches of duty of care.
*   **FRIA as Evidence:** A properly conducted [Fundamental Rights Impact Assessment](../templates/fria-template.md) demonstrates that you anticipated and mitigated risks — this is powerful evidence in defending a liability claim under either the PLD or national tort law.

---

## 5. Key Dates

| Instrument | Key Date | Status |
| :--- | :--- | :--- |
| Revised Product Liability Directive (2024/2853) | **9 December 2026** — national transposition deadline | Adopted. |
| AI Liability Directive (COM/2022/496) | Withdrawn by Commission 16 July 2025; OJ notice **6 October 2025** | **Withdrawn.** No active proposal. |
| EU AI Act — Article 50 transparency | **2 December 2026** under the Digital Omnibus on AI (provisional 7 May 2026); 2 August 2026 pre-Omnibus | In force (phased). |
| EU AI Act — high-risk obligations | **2 December 2027** (Annex III) under the Digital Omnibus on AI (provisional 7 May 2026); 2 August 2026 pre-Omnibus | In force (phased). |

---
*This guide is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 2 — Audit & Procure**, **Step 2.3: Understand AI Liability Exposure**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

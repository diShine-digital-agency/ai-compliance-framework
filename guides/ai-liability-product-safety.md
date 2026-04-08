# AI Liability & Product Safety Guide for the European Market

**Version:** 2.1.0
**Regulatory Context:** April 2026

The EU AI Act defines the *rules* for AI systems, but it does not create a private right of action for individuals harmed by AI. That role falls to two complementary legislative instruments: the **AI Liability Directive** (proposed) and the **revised Product Liability Directive** (Directive 2024/2853). Together with the AI Act, they form a three-pillar regulatory framework for AI in Europe.

This guide explains the liability exposure for enterprises deploying or providing AI systems in the European market.

---

## 1. The Three Pillars of EU AI Regulation

| Pillar | Instrument | Function | Status (April 2026) |
| :--- | :--- | :--- | :--- |
| **Rules** | EU AI Act (Regulation 2024/1689) | Sets obligations for providers, deployers, importers, distributors. Defines prohibited practices and high-risk requirements. | In force. Phased application: prohibited practices (Feb 2025), GPAI (Aug 2025), transparency (Nov 2026), high-risk (Dec 2027). |
| **Fault-Based Liability** | AI Liability Directive (COM/2022/496, proposed) | Facilitates civil liability claims by individuals harmed by AI. Introduces a rebuttable **presumption of causality** and right of **disclosure of evidence**. | Proposed. Under trilogue negotiation as of April 2026. |
| **Strict Liability** | Revised Product Liability Directive (Directive 2024/2853) | Extends product liability to software and AI systems. Enables claims for defective AI products without proving fault. | Adopted December 2024. Member States must transpose by **9 December 2026**. |

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

## 3. The AI Liability Directive (Proposed)

### Status
The AI Liability Directive (COM/2022/496) is a proposed directive intended to complement the revised Product Liability Directive by covering **fault-based** (negligence) claims. As of April 2026, it is under trilogue negotiation. Key provisions:

### A. Presumption of Causality (Article 4)
*   If a provider or deployer **fails to comply** with the EU AI Act (e.g., does not implement required human oversight for a high-risk system), and a claimant suffers damage, the court may **presume** that the non-compliance **caused** the damage.
*   This is a **rebuttable** presumption — the defendant can present evidence to disprove the causal link.
*   **Practical impact:** Non-compliance with the AI Act is not just a regulatory fine risk — it directly increases your civil liability exposure.

### B. Right of Disclosure (Article 3)
*   A potential claimant can request a court to order the provider or deployer to disclose relevant evidence about the AI system (e.g., training data characteristics, logs, audit reports).
*   The court will balance the need for disclosure against trade secret protection.

### C. Scope
*   Covers claims by **any natural person** (not limited to consumers).
*   Applies to both providers and deployers.
*   Complements (does not replace) the Product Liability Directive.

---

## 4. Practical Implications for Enterprises

### For Providers (AI System Developers)
*   **Compliance = Liability Shield:** Strict compliance with the EU AI Act (especially risk management under Article 9, technical documentation under Annex IV, and post-market monitoring under Article 72) directly reduces your exposure under the AI Liability Directive's presumption of causality. See the [Conformity Assessment Guide](../templates/conformity-assessment-guide.md).
*   **Post-Deployment Monitoring:** The revised Product Liability Directive makes you potentially liable for defects introduced by post-deployment learning. Implement robust monitoring and rollback capabilities.
*   **Insurance:** Consider AI-specific product liability insurance. Traditional technology E&O policies may not cover AI system defects.

### For Deployers (AI System Users)
*   **Vendor Contracts:** When using the [Vendor Audit Checklist](../templates/vendor-audit-checklist.md), ensure contracts include:
    *   Clear liability allocation and indemnification for AI system defects.
    *   Right to access logs and technical documentation in the event of a claim.
    *   Vendor obligation to cooperate in court-ordered evidence disclosure.
*   **Human Oversight Documentation:** Document every instance of human oversight for high-risk AI systems. If a court finds that your employees "rubber-stamped" AI decisions without genuine review, the presumption of causality under the AI Liability Directive applies.
*   **FRIA as Evidence:** A properly conducted [Fundamental Rights Impact Assessment](../templates/fria-template.md) demonstrates that you anticipated and mitigated risks — this is powerful evidence in defending a liability claim.

---

## 5. Key Dates

| Instrument | Key Date | Status |
| :--- | :--- | :--- |
| Revised Product Liability Directive (2024/2853) | **9 December 2026** — national transposition deadline | Adopted. |
| AI Liability Directive (COM/2022/496) | TBD — trilogue negotiations ongoing | Proposed. |
| EU AI Act — high-risk obligations | **2 December 2027** (Annex III) | In force (phased). |

---
*This guide is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 2 — Audit & Procure**, **Step 2.3: Understand AI Liability Exposure**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

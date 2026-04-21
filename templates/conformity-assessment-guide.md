# Conformity Assessment Pathway Guide for High-Risk AI Systems

**Version:** 2.1.0
**Regulatory Basis:** EU AI Act Articles 43, 48; Annexes VI, VII

Providers of high-risk AI systems must undergo a **conformity assessment** before placing the system on the EU market or putting it into service. This guide explains when you can self-assess (Internal Control) vs. when you need a Notified Body, and walks through the CE marking process.

---

## 1. Conformity Assessment: Two Pathways

The EU AI Act provides two pathways. Which one you must follow depends on the nature of your high-risk AI system.

### Pathway A: Internal Control (Annex VI)
*   **Who uses this:** Most providers of high-risk AI systems listed under **Annex III** (e.g., AI for recruitment, credit scoring, law enforcement).
*   **What it means:** You (the provider) assess your own system's compliance. No external auditor is required.
*   **Requirements:**
    *   Implement and document a **Quality Management System (QMS)** per Article 17.
    *   Prepare **Technical Documentation** per Annex IV.
    *   Ensure the system complies with all Chapter 2 requirements (Articles 8–15).
    *   Verify compliance through internal testing and review.
    *   Draw up the **EU Declaration of Conformity** (Article 48).
    *   Affix the **CE marking** (Article 48).
    *   Register in the **EU AI Database** (see [Registration Guide](eu-ai-database-registration-guide.md)).

### Pathway B: Third-Party Conformity Assessment via Notified Body (Annex VII)
*   **Who uses this:** Providers of high-risk AI systems that are **safety components of regulated products** under EU harmonisation legislation listed in **Annex I** (e.g., medical devices under MDR, machinery under Machinery Regulation, aviation components). Also required for **biometric identification** systems used by law enforcement under Annex III, Point 1.
*   **What it means:** An independent, accredited **Notified Body** audits your system and issues a certificate of conformity.
*   **Requirements:**
    *   All requirements from Pathway A, **plus**:
    *   Submit the QMS documentation and technical file to the Notified Body.
    *   The Notified Body audits the QMS, reviews the technical documentation, and may test the AI system.
    *   If satisfied, the Notified Body issues a **QMS Certificate** and/or a **Technical Documentation Certificate**.
    *   These certificates are valid for a maximum of **5 years** and must be renewed.

---

## 2. Decision Flowchart: Which Pathway?

```
Is your AI system a safety component of, or itself, a product
covered by EU harmonisation legislation listed in Annex I
(e.g., medical device, machinery, vehicle)?
│
├── YES → Is a third-party conformity assessment already
│         required under that legislation?
│         │
│         ├── YES → Pathway B (Notified Body) — Annex VII
│         │         The AI Act conformity assessment is
│         │         integrated into the existing product
│         │         conformity assessment.
│         │
│         └── NO  → Pathway A (Internal Control) — Annex VI
│
└── NO  → Is the system used for real-time biometric
          identification by law enforcement (Annex III.1)?
          │
          ├── YES → Pathway B (Notified Body) — Annex VII
          │
          └── NO  → Pathway A (Internal Control) — Annex VI
```

---

## 3. The Quality Management System (QMS) — Article 17

Regardless of the pathway, every provider of a high-risk AI system must implement a QMS covering:

*   [ ] **Compliance Strategy:** A documented strategy for regulatory compliance, including conformity assessment procedures.
*   [ ] **Design & Development Controls:** Systematic procedures for the design, development, and testing of the AI system.
*   [ ] **Data Management:** Procedures for data governance, including training data examination, preparation, labelling, and bias management (per Article 10).
*   [ ] **Risk Management:** A risk management system per Article 9, covering known and foreseeable risks, estimation of risks, and adoption of risk management measures.
*   [ ] **Post-Market Monitoring:** A post-market monitoring system per Article 72, including procedures for collecting and analysing data on the AI system's performance throughout its lifecycle.
*   [ ] **Incident Reporting:** Procedures for reporting serious incidents per Article 73 (see the [Incident Response Playbook](ai-incident-response-playbook.md)).
*   [ ] **Communication with Authorities:** Procedures for communication with national competent authorities and the AI Office.
*   [ ] **Record-Keeping:** Systems for document management and record-keeping to demonstrate compliance.
*   [ ] **Resource Management:** Allocation of adequate human and technical resources for AI governance.
*   [ ] **Accountability:** A framework of accountability and responsibility, including clear role assignments.

---

## 4. Technical Documentation (Annex IV)

The technical documentation must include, at minimum the items listed in Annex IV of Regulation (EU) 2024/1689. *Note: check the AI Office website for any officially published documentation templates or implementing acts that national Market Surveillance Authorities may use as audit benchmarks.*

*   [ ] A general description of the AI system and its intended purpose.
*   [ ] A detailed description of the elements and development process, including:
    *   Design specifications, system architecture, and algorithms.
    *   Data requirements (training, validation, and testing datasets).
    *   Development methodology and training approach.
*   [ ] Monitoring, functioning, and control of the AI system, including:
    *   Capabilities and limitations (accuracy, robustness, cybersecurity measures).
    *   Human oversight measures (Article 14).
    *   Logging capabilities (Article 12).
*   [ ] Risk management system documentation (Article 9).
*   [ ] Description of changes made to the system throughout its lifecycle.
*   [ ] Applicable harmonised standards or common specifications used.
*   [ ] EU Declaration of Conformity (Article 47).
*   [ ] Detailed description of the post-market monitoring system (Article 72).

---

## 5. The CE Marking & EU Declaration of Conformity

### EU Declaration of Conformity (Article 47)
The provider draws up a written Declaration of Conformity for each AI system, stating:
*   The name and type of the AI system.
*   The name and address of the provider (and Authorised Representative, if applicable).
*   A statement that the Declaration is issued under the sole responsibility of the provider.
*   A statement that the AI system complies with the EU AI Act and any other applicable Union harmonisation legislation.
*   References to the harmonised standards or common specifications applied.
*   The name and identification number of the Notified Body (if Pathway B).
*   The date, place, and signature of the authorised person.

### CE Marking (Article 48)
*   The CE mark must be affixed **visibly, legibly, and indelibly** to the AI system or its packaging/documentation.
*   If Pathway B was used, the CE mark must be followed by the identification number of the Notified Body.
*   The CE mark must be affixed **before** the system is placed on the market.

---

## 6. Notified Bodies in the EU

Notified Bodies are independent organisations designated by EU Member States to carry out third-party conformity assessments. They must be accredited under Article 28.

*   **Finding a Notified Body:** The EU maintains the [NANDO database](https://ec.europa.eu/growth/tools-databases/nando/) listing all notified bodies and their designated scope.
*   **AI-specific accreditation:** As of April 2026, the designation of AI Act-specific Notified Bodies is ongoing in most Member States. For AI systems that are *also* medical devices or other regulated products, existing Notified Bodies under MDR/IVDR/Machinery Regulation may be extended to cover AI Act obligations.

---

## 7. Timeline

| Milestone | Deadline |
| :--- | :--- |
| Transparency/Art. 50 systems | **2 November 2026** |
| High-risk systems — Annex III (standalone) | **2 December 2027** |
| High-risk systems — regulated products (Art. 6.1) | **2 August 2028** |

---
*This guide is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 3 — Architect & Deploy**, **Step 3.7: Conformity Assessment & CE Marking**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

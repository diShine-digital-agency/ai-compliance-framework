# AI Vendor Due Diligence

When an organisation procures AI capabilities from a third-party vendor — whether as a cloud API, SaaS platform, or embedded component — it must conduct thorough due diligence to ensure the vendor meets GDPR, EU AI Act, and security requirements.

Standard security questionnaires (SOC 2, ISO 27001) are necessary but **insufficient** for AI vendors. AI introduces specific risks around training data provenance, automated decision-making, model behaviour, and regulatory classification that standard procurement frameworks do not cover.

## Why AI Vendor Due Diligence Is Different

| Standard Vendor Audit | AI-Specific Addition |
|---|---|
| Data processing agreement | Training data opt-out, model improvement restrictions |
| Data residency | Inference-time data routing, model hosting location |
| Sub-processors | Upstream model providers (e.g., OpenAI, Anthropic, Google) |
| Security controls | Prompt injection defences, model isolation, adversarial robustness |
| Compliance certifications | EU AI Act risk classification, conformity assessment status |
| Incident response | AI-specific incident taxonomy (bias discovery, model inversion, hallucination) |

## The 25-Point Audit Framework

The repository's [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) provides a structured 25-point assessment organised in three parts:

### Part 1: GDPR Compliance (Items 1–10)

| Item | Focus Area |
|---|---|
| 1 | Data Processing Agreement (DPA) with Article 28 required clauses |
| 2 | Training data — does the vendor use customer data for model training? |
| 3 | Data retention and deletion policies |
| 4 | Data residency — where is data stored and processed? |
| 5 | International transfers — Standard Contractual Clauses, adequacy decisions |
| 6 | Sub-processors — who are they? How are they controlled? |
| 7 | GDPR Article 22 — automated decision-making safeguards |
| 8 | Data subject rights — can you fulfil access, rectification, erasure requests? |
| 9 | DPIA — has the vendor conducted one? Will they share it? |
| 10 | Breach notification — vendor's procedure and timeline |

### Part 2: EU AI Act Compliance (Items 11–20)

| Item | Focus Area |
|---|---|
| 11 | Risk classification — has the vendor classified its system? |
| 12 | For high-risk systems: conformity assessment status |
| 13 | Technical documentation (Annex IV) availability |
| 14 | Human oversight — what mechanisms are built in? |
| 15 | Accuracy and robustness — documented performance metrics |
| 16 | Bias testing — what fairness evaluations have been conducted? |
| 17 | Transparency — Article 50 compliance for chatbots, deepfakes |
| 18 | GPAI model obligations (Articles 53–55) — copyright policy, training data summary |
| 19 | Post-market monitoring — vendor's monitoring programme |
| 20 | Serious incident reporting — vendor's procedure and commitments |

### Part 3: Security and IP (Items 21–25)

| Item | Focus Area |
|---|---|
| 21 | Prompt injection defences — input sanitisation, output filtering |
| 22 | Model isolation — is your data segregated from other customers? |
| 23 | IP rights — who owns outputs? What are the licensing terms? |
| 24 | Content filtering — what safety filters are applied? |
| 25 | Sub-processor and upstream model provider transparency |

## Scoring and Assessment

The [Interactive Compliance Toolkit](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/tools/compliance-toolkit.html) includes a **Vendor Compliance Scorecard** that tracks progress against all 25 items and generates a compliance grade:

| Grade | Score | Meaning |
|---|---|---|
| **A** | 90–100% | Full compliance; vendor meets all requirements |
| **B** | 75–89% | Mostly compliant; minor gaps to address |
| **C** | 60–74% | Significant gaps; remediation plan required before deployment |
| **D** | Below 60% | Non-compliant; do not proceed without substantial vendor changes |

## Key Red Flags

During vendor assessment, watch for these warning signs:

1. **"We can't share our DPA"** — every AI vendor processing personal data on your behalf must have a DPA.
2. **No training data opt-out** — consumer-tier AI services that use customer data for model training are unsuitable for enterprise use.
3. **Unclear data residency** — if the vendor cannot confirm where data is processed, you cannot ensure GDPR compliance for international transfers.
4. **No risk classification** — vendors who have not assessed their AI system against the EU AI Act risk categories may not be compliance-ready.
5. **No bias testing** — for high-risk applications (HR, credit, insurance), the absence of fairness evaluation is a significant gap.
6. **Opaque sub-processor chain** — if the vendor uses upstream AI providers (e.g., a SaaS company that uses OpenAI's API), the sub-processor chain must be documented and assessed.

## Contract Clauses

Key provisions to include in AI vendor contracts:

- **Training data restriction** — contractual prohibition on using customer data for model training
- **Data residency** — specified processing locations with notification of changes
- **Audit rights** — right to audit or inspect the vendor's AI compliance measures
- **Compliance representations** — vendor represents compliance with GDPR and EU AI Act
- **Incident notification** — specified timeframes for breach and incident notification
- **Indemnification** — allocation of liability for AI-related harms
- **Exit provisions** — data return/deletion and model disengagement procedures

## Vendor Assessment in the Framework Journey

Vendor due diligence sits in **Phase 2 (Audit & Procure)** of the framework's [Step-by-Step User Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/how-to-use-this-framework.md):

1. Phase 1 (Assess & Contain): Establish policies and assess Shadow AI exposure
2. **Phase 2 (Audit & Procure): Audit existing vendors; apply sector-specific rules**
3. Phase 3 (Architect & Deploy): Choose deployment tiers, conduct assessments
4. Phase 4 (Monitor & Respond): Ongoing monitoring and incident response

---

**See also:** [Shadow AI: Risks and Mitigation](Shadow-AI) · [GDPR and AI](GDPR-and-AI) · [EU AI Act Roles](EU-AI-Act-Roles) · [General Purpose AI (GPAI)](General-Purpose-AI-GPAI) · [Home](Home)

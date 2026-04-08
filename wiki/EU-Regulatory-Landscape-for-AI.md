# EU Regulatory Landscape for AI

The EU AI Act does not exist in isolation. It is part of a broader regulatory ecosystem that together governs how organisations develop, deploy, and operate AI systems in the European Union. Understanding the interplay between these regulations is essential for building a comprehensive compliance programme.

## The Regulatory Stack

```
┌─────────────────────────────────────────────────────────────────────┐
│                    EU AI Act (2024/1689)                            │
│            Risk-based AI-specific requirements                      │
├───────────────────────┬────────────────────────┬────────────────────┤
│   GDPR (2016/679)     │   NIS2 (2022/2555)     │   CRA (2024/2847)  │
│   Data protection     │   Cybersecurity for     │   Product cyber-   │
│                       │   essential entities     │   security         │
├───────────────────────┼────────────────────────┼────────────────────┤
│   DORA (2022/2554)    │   PLD (2024/2853)      │   AILD (proposed)  │
│   Financial sector    │   Product liability     │   AI-specific      │
│   resilience          │   (strict)              │   liability (fault)│
├───────────────────────┼────────────────────────┼────────────────────┤
│   DSA (2022/2065)     │   DMA (2022/1925)      │                    │
│   Platform content    │   Digital market        │                    │
│   & algorithms        │   gatekeepers           │                    │
└───────────────────────┴────────────────────────┴────────────────────┘
```

## Regulation-by-Regulation Summary

### 1. General Data Protection Regulation (GDPR)

| | |
|---|---|
| **In force since** | 25 May 2018 |
| **Scope** | All processing of personal data |
| **Maximum penalty** | €20 million / 4% of global turnover |
| **AI-specific relevance** | Lawful basis for training data, DPIA for AI systems, Article 22 automated decision-making, breach notification |

See [GDPR and AI](GDPR-and-AI) for a detailed analysis.

### 2. NIS2 Directive (2022/2555)

| | |
|---|---|
| **In force since** | 16 January 2023; transposition deadline 17 October 2024 |
| **Scope** | Essential and important entities in critical sectors (energy, transport, banking, health, digital infrastructure, ICT service management, public administration, space, food, manufacturing, digital providers) |
| **Maximum penalty** | €10 million / 2% of turnover (essential entities); €7 million / 1.4% (important entities) |
| **AI-specific relevance** | Risk management for networked systems running AI; supply chain cybersecurity due diligence; **24-hour** initial incident notification, followed by a **72-hour** detailed report |

**Key overlap with AI Act:**
- Both require risk management and incident reporting, but with different timelines and authorities.
- NIS2 mandates cybersecurity for the infrastructure running AI systems; the AI Act mandates cybersecurity of the AI system itself (Article 15).
- Supply chain requirements under NIS2 complement AI Act vendor due diligence.

### 3. Digital Operational Resilience Act (DORA, 2022/2554)

| | |
|---|---|
| **In force since** | 16 January 2023; applies from 17 January 2025 |
| **Scope** | Financial sector — credit institutions, investment firms, insurance undertakings, payment institutions, crypto-asset service providers, and their ICT third-party service providers |
| **Maximum penalty** | Up to €10 million / 5% of turnover for credit institutions; penalties for ICT third-party providers determined by the Lead Overseer |
| **AI-specific relevance** | ICT risk management covering AI-based services; incident classification and reporting; third-party risk management for AI vendors; digital operational resilience testing |

**Key overlap with AI Act:**
- Financial institutions using AI for credit scoring or insurance pricing face concurrent obligations under DORA (operational resilience), the AI Act (high-risk system requirements), and GDPR (automated decision-making).
- An AI-driven security breach in a bank might trigger different notification duties under DORA (within hours), GDPR (72 hours), and the AI Act (15 days), to different authorities.

See [Sector Guide: Financial Services](Sector-Guide-Financial-Services).

### 4. Cyber Resilience Act (CRA, 2024/2847)

| | |
|---|---|
| **Adopted** | October 2024; obligations phase in through 2027 |
| **Scope** | Products with digital elements (hardware and software) placed on the EU market, including embedded AI |
| **Maximum penalty** | €15 million / 2.5% of global turnover |
| **AI-specific relevance** | Security-by-design requirements for AI-enabled products; vulnerability disclosure obligations; lifecycle security updates; CE marking for cybersecurity |

**Key overlap with AI Act:**
- AI-enabled products may require compliance with both the CRA (cybersecurity requirements) and the AI Act (AI-specific requirements).
- Documentation, testing, and conformity assessment obligations may overlap or be redundant.
- The CRA focuses on the product's cybersecurity; the AI Act focuses on the AI system's safety, transparency, and fundamental rights impact.

See [Sector Guide: Technology](Sector-Guide-Technology).

### 5. Product Liability Directive (PLD, 2024/2853)

| | |
|---|---|
| **Adopted** | November 2024; transposition deadline December 2026 |
| **Scope** | All products placed on the EU market, explicitly including software and AI systems |
| **Liability type** | **Strict liability** — the injured party does not need to prove fault, only that the product was defective and caused the damage |
| **AI-specific relevance** | AI systems and their outputs are explicitly covered as "products"; non-compliance with the AI Act may constitute evidence of defectiveness; burden of proof lightening for claimants |

### 6. AI Liability Directive (AILD, proposed — COM/2022/496)

| | |
|---|---|
| **Status** | Proposed by the Commission in September 2022; legislative process ongoing |
| **Scope** | Fault-based civil liability claims involving AI systems |
| **Liability type** | **Fault-based** but with **presumption of causality** — if a defendant violated a duty of care (such as non-compliance with the AI Act), and the damage is the kind that the duty was designed to prevent, causality is presumed |
| **AI-specific relevance** | Makes it easier for claimants to bring civil liability claims against AI providers and deployers; the "black box" problem is addressed through disclosure obligations |

See [AI Liability in the EU](AI-Liability-in-the-EU) for a comprehensive analysis of the three-pillar liability framework.

### 7. Digital Services Act (DSA, 2022/2065)

| | |
|---|---|
| **In force since** | 16 November 2022; applies fully since 17 February 2024 |
| **Scope** | Intermediary services, hosting services, online platforms, very large online platforms (VLOPs) and very large online search engines (VLOSEs) with 45+ million monthly EU users |
| **Maximum penalty** | 6% of global annual turnover for VLOPs/VLOSEs |
| **AI-specific relevance** | Algorithmic transparency for recommender systems; content moderation by AI; systemic risk assessments for AI-driven platforms; user rights regarding algorithmic recommendations |

**Key overlap with AI Act:**
- Both regulate AI-powered content moderation and recommender systems, but the DSA focuses on platform obligations while the AI Act focuses on system-level requirements.
- VLOPs must conduct annual systemic risk assessments covering AI-driven content amplification, manipulation of public discourse, and impacts on fundamental rights.
- VLOPs must provide users with at least one non-profiling-based recommender system option.
- Content moderation AI must be transparent — platforms must explain how automated tools flag, remove, or deprioritise content.
- The DSA Digital Services Coordinator in each Member State may need to coordinate with the AI Act market surveillance authority.

## Incident Reporting — A Comparison

One of the most practical compliance challenges is managing overlapping incident reporting obligations:

| Regulation | Trigger | Deadline | Report To |
|---|---|---|---|
| **GDPR** | Personal data breach | **72 hours** | National Data Protection Authority |
| **NIS2** | Significant cybersecurity incident | **24 hours** (initial), **72 hours** (detailed) | National CSIRT/competent authority |
| **DORA** | Major ICT-related incident | **4 hours** (initial), **72 hours** (intermediate), **1 month** (final) | National financial supervisor |
| **EU AI Act** | Serious incident involving high-risk AI | **15 days** | National market surveillance authority |

A single AI-related incident (e.g., a prompt injection attack on a financial institution's AI chatbot that exposes customer data) could trigger reporting obligations under all four regimes simultaneously, each with different timelines, content requirements, and recipient authorities.

The repository's [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) addresses multi-regime incident reporting.

## Building a Unified Compliance Programme

The AI Compliance Framework repository is designed to help organisations manage these overlapping obligations through integrated templates:

| Cross-Cutting Need | Framework Template |
|---|---|
| Risk assessment (GDPR + AI Act) | [DPIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) + [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) |
| Vendor due diligence (GDPR + AI Act + NIS2) | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) |
| Incident management (GDPR + AI Act + NIS2 + DORA) | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |
| Governance framework (AI Act + ISO 42001) | [ISO 42001 Alignment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/iso42001-alignment-guide.md) |
| Financial services specifics (AI Act + DORA + MiFID II) | [Sector Addendum: Finance](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-finance.md) |
| Technology sector specifics (AI Act + NIS2 + CRA) | [Sector Addendum: Technology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-tech.md) |

---

**See also:** [GDPR and AI](GDPR-and-AI) · [AI Liability in the EU](AI-Liability-in-the-EU) · [EU AI Act Overview](EU-AI-Act-Overview) · [National Implementation by Member States](National-Implementation) · [Transparency Obligations (Article 50)](Transparency-Obligations) · [Home](Home)

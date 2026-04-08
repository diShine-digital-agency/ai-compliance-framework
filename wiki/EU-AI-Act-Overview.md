# EU AI Act Overview

The EU AI Act — formally Regulation (EU) 2024/1689 — is the world's first comprehensive legal framework for artificial intelligence. It was adopted by the European Parliament and the Council of the European Union and published in the Official Journal on 12 July 2024. It entered into force on 1 August 2024, with obligations phasing in between February 2025 and August 2027.

## Legislative History

| Date | Event |
|------|-------|
| April 2021 | European Commission publishes the original legislative proposal |
| December 2023 | European Parliament and Council reach political agreement |
| 13 March 2024 | European Parliament adopts the final text |
| 21 May 2024 | Council of the EU formally adopts the Regulation |
| 12 July 2024 | Published in the Official Journal of the EU |
| 1 August 2024 | Entry into force (20 days after publication) |

## Objectives

The AI Act has three stated objectives:

1. **Protecting fundamental rights and safety** — ensuring AI systems placed on the EU market or used within the EU do not undermine human dignity, non-discrimination, privacy, or other rights enshrined in the EU Charter of Fundamental Rights.
2. **Creating legal certainty** — providing a single, harmonised regulatory framework across all 27 Member States, replacing the prior patchwork of national approaches and voluntary guidelines.
3. **Supporting innovation** — establishing proportionate obligations calibrated to risk, so that low-risk AI applications face minimal regulatory burden while high-risk systems receive appropriate oversight.

## Scope

The AI Act applies to:

- **Providers** (developers) of AI systems that are placed on the EU market or put into service in the EU, regardless of where the provider is established.
- **Deployers** (users) of AI systems located within the EU.
- **Importers and distributors** of AI systems in the EU.
- **Providers and deployers outside the EU**, when the output of their AI system is used within the EU.

It does **not** apply to:
- AI systems used exclusively for military, defence, or national security purposes.
- AI systems used solely for scientific research and development before market placement.
- AI systems released under free and open-source licences (with exceptions for high-risk and prohibited systems).
- Personal, non-professional use of AI by natural persons.

## Structure

The Act is structured around a **risk-based classification system** (see [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification)):

| Risk Level | Regulatory Treatment |
|------------|---------------------|
| **Unacceptable** | Prohibited outright |
| **High** | Permitted but subject to strict requirements and conformity assessment |
| **Limited** | Transparency obligations only |
| **Minimal** | No specific obligations (voluntary codes of conduct encouraged) |

## Key Provisions

### Prohibited AI Practices (Article 5)
Certain AI applications are banned entirely because they pose an unacceptable risk to fundamental rights. These include social scoring, subliminal manipulation, exploitation of vulnerabilities, real-time remote biometric identification in public spaces (with limited exceptions), emotion recognition in workplaces and schools, and untargeted facial image scraping. See [Prohibited AI Practices](Prohibited-AI-Practices).

### High-Risk AI Systems (Articles 6–15, Annex III)
AI systems used in specified sensitive domains (employment, education, critical infrastructure, law enforcement, migration, administration of justice, credit scoring, biometric identification) are classified as high-risk and must comply with requirements for risk management, data governance, technical documentation, transparency, human oversight, accuracy, robustness, and cybersecurity. See [High-Risk AI Systems](High-Risk-AI-Systems).

### General Purpose AI (Articles 51–55)
Models capable of performing a wide range of tasks (such as large language models) are subject to transparency and documentation obligations. Those exceeding the 10²⁵ FLOP training compute threshold are classified as posing systemic risk, with additional obligations for adversarial testing and incident reporting. See [General Purpose AI (GPAI)](General-Purpose-AI-GPAI).

### Transparency Obligations (Article 50)
AI systems that interact directly with people (chatbots), generate synthetic content (deepfakes), or perform emotion recognition or biometric categorisation must disclose that fact to the user.

### Conformity Assessment (Articles 43–49)
Before a high-risk AI system can be placed on the market, the provider must demonstrate compliance through either internal control (self-assessment) or third-party assessment by a Notified Body. See [Conformity Assessment](Conformity-Assessment).

### EU AI Database (Article 49)
High-risk AI systems must be registered in the EU AI Database before market placement. See [EU AI Database Registration](EU-AI-Database-Registration).

### Fundamental Rights Impact Assessment (Article 27)
Deployers of high-risk AI systems in specific categories must conduct an FRIA before deployment. See [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment).

### AI Literacy (Article 4)
All providers and deployers must ensure that their staff and other persons dealing with the operation and use of AI systems have a sufficient level of AI literacy. This obligation has applied since 2 February 2025. See [AI Literacy Obligation](AI-Literacy-Obligation).

### Penalties (Article 99)
The Act establishes a three-tier penalty structure with maximum fines of €35 million / 7% turnover, €15 million / 3% turnover, and €7.5 million / 1% turnover. See [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines).

## Governance Architecture

The AI Act establishes a multi-level governance structure:

- **European AI Office** — housed within the European Commission, responsible for oversight of GPAI models, coordinating enforcement, and issuing guidelines. Operational since August 2025.
- **European Artificial Intelligence Board** — composed of representatives from each Member State, ensures harmonised application across the EU.
- **National Market Surveillance Authorities** — designated by each Member State, responsible for enforcement at the national level. See [National Implementation by Member States](National-Implementation).
- **Notified Bodies** — independent conformity assessment bodies accredited to evaluate high-risk AI systems.

## Relationship to Other Legislation

The AI Act does not operate in isolation. It interacts with:

- **GDPR** — personal data processing by AI systems remains subject to GDPR. See [GDPR and AI](GDPR-and-AI).
- **Product Liability Directive** and **AI Liability Directive** — non-compliance with the AI Act can trigger liability presumptions. See [AI Liability in the EU](AI-Liability-in-the-EU).
- **NIS2, DORA, and the Cyber Resilience Act** — overlapping cybersecurity and operational resilience requirements. See [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI).
- **Sector-specific legislation** — MDR/IVDR (medical devices), MiFID II (financial instruments), DORA (financial sector resilience).

## How This Framework Helps

The AI Compliance Framework repository provides practical templates that operationalise the AI Act's requirements:

| AI Act Requirement | Framework Template |
|---|---|
| Article 4 (AI Literacy) | [AI Literacy Programme](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-literacy-programme.md) |
| Article 5 (Prohibited Practices) | [Acceptable AI Use Policy](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/acceptable-use-policy.md) |
| Articles 9–15 (High-Risk Requirements) | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md), [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md) |
| Article 27 (FRIA) | [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) |
| Articles 43–49 (Conformity Assessment) | [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md), [EU AI Database Registration Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/eu-ai-database-registration-guide.md) |
| Articles 53–55 (GPAI) | [GPAI Model Governance Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/gpai-model-governance-checklist.md) |
| Article 73 (Incident Reporting) | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |

---

**See also:** [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification) · [EU AI Act Enforcement Timeline](EU-AI-Act-Enforcement-Timeline) · [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines) · [Home](Home)

# General Purpose AI (GPAI)

General-Purpose AI (GPAI) models — including large language models such as GPT, Claude, Gemini, Llama, and Mistral — are subject to specific obligations under the EU AI Act. These obligations have been in force since **2 August 2025**.

## What Is a GPAI Model

The EU AI Act defines a GPAI model (Article 3(63)) as an AI model that:
- Is trained with a large amount of data using self-supervision at scale
- Displays significant generality
- Is capable of competently performing a wide range of distinct tasks regardless of the way it is placed on the market
- Can be integrated into a variety of downstream systems or applications

This definition is technology-neutral but in practice covers foundation models, large language models, and multimodal models.

## Two Categories of GPAI

The Act distinguishes between:

### 1. Standard GPAI Models (Article 53)

All GPAI models must comply with **baseline transparency and documentation obligations**.

### 2. GPAI Models with Systemic Risk (Articles 51, 55)

A GPAI model is classified as posing **systemic risk** if:
- It has **high impact capabilities**, which is presumed when the cumulative amount of compute used for training exceeds **10²⁵ floating point operations (FLOPs)**, or
- The European Commission designates it as such, based on criteria in Annex XIII

Models with systemic risk have additional obligations beyond the baseline.

## Baseline Obligations — All GPAI Models (Article 53)

| Obligation | Description |
|------------|-------------|
| **Technical documentation** | Draw up and maintain technical documentation of the model, including training and testing processes, evaluation results, and information about the model's capabilities and limitations. Must be provided to the AI Office and national authorities on request. |
| **Information to downstream providers** | Provide sufficient information and documentation to downstream AI system providers to enable them to understand the model's capabilities and comply with their own obligations. Must be provided within 14 days of request. |
| **Copyright policy** | Put in place a policy to comply with EU copyright law, in particular regarding the text and data mining exception (Article 4 of Directive (EU) 2019/790). Must maintain and publish a sufficiently detailed summary of the training data content. |
| **Training data summary** | Draw up and make publicly available a sufficiently detailed summary of the content used for training, following a template provided by the AI Office. |

## Additional Obligations — Systemic Risk Models (Article 55)

| Obligation | Description |
|------------|-------------|
| **Model evaluation** | Perform model evaluations, including adversarial testing, to identify and mitigate systemic risks, with attention to risks identified by the scientific panel of independent experts. |
| **Systemic risk assessment and mitigation** | Assess and mitigate possible systemic risks at EU level, including their sources. |
| **Incident tracking and reporting** | Track, document, and report serious incidents and possible corrective measures to the AI Office and, where relevant, to national authorities without undue delay. |
| **Adequate cybersecurity** | Ensure an adequate level of cybersecurity for the model and its physical infrastructure. |

## The GPAI Code of Practice

The final **GPAI Code of Practice** was published on **10 July 2025**. It provides a voluntary but influential framework for demonstrating compliance with Articles 53 and 55.

### Structure

The Code is organised into three chapters:

1. **Transparency** — standardised Model Documentation Form, detailed disclosures covering licensing, use cases, datasets, compute requirements, capabilities, and limitations.
2. **Copyright** — copyright compliance policies, procedures for responding to opt-out requests under the text and data mining exception.
3. **Safety & Security** — advanced risk management procedures for systemic risk models, including risk identification frameworks, safety mitigations, model evaluations, and incident reporting.

### Legal Status

- Joining the Code is **voluntary**.
- Adherence provides a **rebuttable presumption of compliance** with the corresponding AI Act obligations. This means that if a provider demonstrates compliance with the Code, it is presumed to comply with the relevant statutory obligations unless evidence to the contrary is presented.
- Providers who do not join the Code must independently demonstrate compliance, which typically involves greater regulatory scrutiny.

### Enforcement

- Enforcement actions by the European Commission (model recalls, information requests) for GPAI obligations become available from **2 August 2026**.
- GPAI models placed on the market before 2 August 2025 must be brought into compliance by **2 August 2027**.

## Provider vs. Deployer Obligations for GPAI

### GPAI Model Provider
- Must comply with Article 53 (all models) and Article 55 (systemic risk models).
- Must provide downstream providers and deployers with sufficient documentation and information.

### Downstream AI System Provider (Integrator)
- When integrating a GPAI model into a specific AI system (e.g., building a recruitment tool on top of GPT-4), the integrator becomes the **provider** of the resulting AI system and must comply with all obligations applicable to that system's risk classification.
- Can rely on documentation and information provided by the GPAI model provider but retains responsibility for the final system's compliance.

### Deployer
- Must ensure AI literacy (Article 4) and, if the system is high-risk, comply with deployer obligations (Article 26).
- Should conduct due diligence on the GPAI model provider's compliance during procurement. The repository's [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) covers GPAI-specific audit items.

## The 10²⁵ FLOP Threshold

The systemic risk threshold is set at **10²⁵ floating point operations** of cumulative compute used for training. For reference:

- GPT-4 (2023) is estimated to have been trained at approximately 10²⁵ FLOP, placing it at the threshold.
- Most open-source models currently available (Llama 2 70B, Mistral 7B) fall below this threshold.
- As compute costs decline and model sizes grow, more models are expected to cross this threshold over time.

The European Commission has the power to update this threshold through delegated acts.

## Framework Templates for GPAI

| Need | Template |
|------|----------|
| GPAI compliance checklist | [GPAI Model Governance Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/gpai-model-governance-checklist.md) |
| Vendor audit for GPAI providers | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) |
| Incident response for GPAI-related issues | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |
| Understanding provider/deployer roles | [Sector Guide: Technology](Sector-Guide-Technology) |

---

**See also:** [EU AI Act Overview](EU-AI-Act-Overview) · [EU AI Act Roles](EU-AI-Act-Roles) · [AI Vendor Due Diligence](AI-Vendor-Due-Diligence) · [Home](Home)

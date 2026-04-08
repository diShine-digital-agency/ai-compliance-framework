# Sector Guide: Healthcare

Healthcare AI sits at the intersection of the EU AI Act and the Medical Devices Regulation (MDR 2017/745) / In Vitro Diagnostic Medical Devices Regulation (IVDR 2017/746). If an AI system qualifies as a medical device, it is **automatically high-risk** under the AI Act.

## When Is Healthcare AI a Medical Device?

An AI system is a medical device if it has a **medical purpose** as defined by the MDR:
- Diagnosis, prevention, monitoring, prediction, prognosis, treatment, or alleviation of disease
- Investigation, replacement, or modification of anatomy or a physiological or pathological process

| AI Application | Likely Medical Device? | AI Act Classification |
|---|---|---|
| **Diagnostic imaging AI** (radiology, pathology) | Yes | High-risk (Annex I product + Annex III) |
| **Clinical Decision Support Systems (CDSS)** | Often yes (depends on intended purpose) | High-risk |
| **Triage chatbots** (symptom checkers) | Possibly (if directing clinical decisions) | High-risk or limited risk |
| **Drug discovery / molecular modelling** | Generally no (research tool, not clinical) | Typically minimal risk |
| **Hospital resource optimisation** | No (operational, not diagnostic) | Generally not high-risk |
| **Patient scheduling** | No | Minimal risk |
| **Wellness apps** (general fitness tracking) | No (unless making diagnostic claims) | Minimal or limited risk |

## Dual Regulatory Burden

Healthcare AI that qualifies as a medical device must comply with both:

### MDR/IVDR Requirements
- Conformity assessment by a Notified Body (for Class IIa and above devices)
- Technical documentation per Annex II/III of the MDR
- Quality management system per ISO 13485
- Post-market surveillance
- Clinical evaluation / performance evaluation
- Unique Device Identification (UDI)

### AI Act Requirements
- Risk management system (Article 9)
- Data governance (Article 10) — particular attention to health data under GDPR Article 9
- Technical documentation (Annex IV)
- Human oversight (Article 14) — critical for clinical decisions
- Accuracy, robustness, cybersecurity (Article 15)
- The conformity assessment follows the **MDR/IVDR pathway** (not the AI Act standalone pathway)

## GDPR Article 9 — Health Data

Health data is special category data under GDPR Article 9. Processing is generally prohibited unless an exception applies:

| Exception | Application in Healthcare AI |
|---|---|
| **Explicit consent** (Art. 9(2)(a)) | Patient consent for AI-assisted diagnosis — must be freely given, specific, informed |
| **Healthcare provision** (Art. 9(2)(h)) | Processing necessary for medical diagnosis, provision of healthcare, treatment — under the responsibility of a healthcare professional bound by professional secrecy |
| **Public health** (Art. 9(2)(i)) | Processing necessary for public interest in the area of public health |
| **Scientific research** (Art. 9(2)(j)) | Subject to appropriate safeguards (pseudonymisation, data minimisation) |

## Human Oversight in Clinical AI

Article 14 of the AI Act requires human oversight for high-risk systems. In healthcare, this translates to:

- **AI systems should support, not replace, clinical decision-making.** The clinician retains responsibility for the final decision.
- **Clinicians must be able to understand the AI's output** — explainability is essential for clinical trust and regulatory compliance.
- **Clinicians must be able to override the AI** — the system must allow the clinician to deviate from the AI recommendation without technical barriers.
- **Training** — clinicians using AI systems must understand the system's capabilities, limitations, and potential failure modes (AI literacy obligation, Article 4).

## Algorithmic Bias in Healthcare

Healthcare AI carries particular bias risks:

- **Training data imbalance** — medical datasets may underrepresent certain populations (e.g., skin conditions in darker skin tones, gender-specific disease presentations)
- **Historical treatment disparities** — models trained on historical clinical data may perpetuate disparities in care access and treatment quality
- **Socioeconomic proxies** — variables correlated with socioeconomic status may bias triage and resource allocation decisions

The [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) provides the audit framework applicable to healthcare AI.

## Framework Template

The repository's [Healthcare & Life Sciences Sector Addendum](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-healthcare.md) covers:
- MDR/IVDR regulatory mapping
- CDSS classification guidance
- GDPR Article 9 exception mapping
- Data governance for health data
- Human oversight requirements for clinical AI

---

**See also:** [High-Risk AI Systems](High-Risk-AI-Systems) · [Conformity Assessment](Conformity-Assessment) · [GDPR and AI](GDPR-and-AI) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [Home](Home)

# GDPR and AI

The General Data Protection Regulation (Regulation (EU) 2016/679) remains the foundational data protection law in the EU. Any AI system that processes personal data must comply with the GDPR, regardless of its risk classification under the EU AI Act.

## Where GDPR and AI Intersect

### Lawful Basis for Processing (Article 6)

Every AI system processing personal data requires a valid lawful basis. The six lawful bases are:

| Lawful Basis | AI Application |
|---|---|
| **Consent** (Art. 6(1)(a)) | Rarely practical for AI training at scale; must be freely given, specific, informed, and unambiguous; can be withdrawn at any time |
| **Contractual necessity** (Art. 6(1)(b)) | May apply when AI processing is necessary to fulfil a contract with the data subject (e.g., personalised service delivery) |
| **Legal obligation** (Art. 6(1)(c)) | Applies when AI processing is required by law (e.g., anti-money laundering screening) |
| **Vital interests** (Art. 6(1)(d)) | Emergency medical AI applications |
| **Public interest** (Art. 6(1)(e)) | Government AI systems (law enforcement, public health) |
| **Legitimate interests** (Art. 6(1)(f)) | The most commonly invoked basis for commercial AI, but requires a balancing test against the data subject's rights |

### Special Category Data (Article 9)

AI systems that process **special category data** (racial or ethnic origin, political opinions, religious beliefs, trade union membership, genetic data, biometric data, health data, sex life or sexual orientation) face additional restrictions. Processing is generally prohibited unless a specific exception applies:

- Explicit consent
- Employment, social security, and social protection law obligations
- Vital interests
- Substantial public interest
- Medical diagnosis or treatment
- Public health
- Archiving, research, or statistics

This is particularly relevant for AI in healthcare (see [Sector Guide: Healthcare](Sector-Guide-Healthcare)) and HR (see [Sector Guide: Human Resources](Sector-Guide-Human-Resources)).

### Automated Decision-Making (Article 22)

Article 22 gives data subjects the right **not to be subject to a decision based solely on automated processing**, including profiling, which produces legal effects or similarly significantly affects them.

**Exceptions** exist where the decision is:
- Necessary for a contract
- Authorised by EU or Member State law
- Based on explicit consent

**When an exception applies**, the data controller must implement **suitable safeguards**, including:
- The right to obtain human intervention
- The right to express their point of view
- The right to contest the decision

This is directly relevant to AI systems used for credit scoring, recruitment, insurance pricing, and benefit eligibility — all of which are also high-risk under the EU AI Act.

### Data Protection Impact Assessment (Article 35)

A DPIA is **mandatory** when processing is likely to result in a **high risk** to the rights and freedoms of natural persons. AI systems frequently trigger this requirement, particularly when involving:

- Systematic and extensive evaluation of personal aspects (profiling)
- Large-scale processing of special category data
- Systematic monitoring of publicly accessible areas
- New technologies (AI/ML qualifies)

The repository provides an [AI-specific DPIA template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) and a [DPIA Example Library](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-example-library.md) with three pre-filled examples. See also [DPIA for AI](DPIA-for-AI).

### Data Protection by Design and by Default (Article 25)

AI systems must incorporate data protection principles from the design stage:

- **Data minimisation** — only process personal data that is necessary for the specific purpose
- **Purpose limitation** — data collected for one purpose cannot be repurposed for AI training without a compatible legal basis
- **Storage limitation** — personal data used for training must be deleted or anonymised when no longer needed
- **Accuracy** — models trained on inaccurate data can perpetuate errors that affect data subjects

### Data Subject Rights

Data subjects retain all GDPR rights when their data is processed by AI systems:

| Right | AI Implication |
|---|---|
| **Right of access** (Art. 15) | Data subjects can request information about what data is being processed and how |
| **Right to rectification** (Art. 16) | Inaccurate data used in AI decisions must be corrected |
| **Right to erasure** (Art. 17) | Data subjects can request deletion; implications for model retraining |
| **Right to restriction** (Art. 18) | Processing can be restricted while accuracy is contested |
| **Right to data portability** (Art. 20) | Data subjects can obtain their data in a structured, machine-readable format |
| **Right to object** (Art. 21) | Data subjects can object to processing based on legitimate interests, including profiling |
| **Right to explanation** (Recital 71) | Although not a standalone right in the GDPR, Recital 71 references the right to obtain "meaningful information about the logic involved" in automated decisions |

### Breach Notification (Articles 33–34)

When an AI system breach involves personal data:
- The **supervisory authority** must be notified within **72 hours** of becoming aware (Article 33)
- If the breach is likely to result in a high risk to individuals, the **data subjects** must also be notified without undue delay (Article 34)

Note: The EU AI Act has a separate **15-day** serious incident reporting requirement (Article 73) for high-risk AI systems. Both timelines may apply simultaneously. See [AI Incident Response](AI-Incident-Response).

## GDPR and EU AI Act: Complementary Obligations

| Obligation | GDPR | EU AI Act |
|---|---|---|
| Risk assessment | DPIA (Art. 35) | Risk management system (Art. 9) + FRIA (Art. 27) |
| Documentation | Records of processing (Art. 30) | Technical documentation (Art. 11, Annex IV) |
| Transparency | Privacy notice (Arts. 13–14) | Information to deployers (Art. 13) + user-facing transparency (Art. 50) |
| Human oversight | Art. 22 safeguards | Human oversight measures (Art. 14) |
| Breach notification | 72-hour DPA notification | 15-day serious incident reporting |
| Accountability | Data controller responsibility | Provider/deployer obligations |

Both laws apply concurrently. Compliance with one does not exempt from the other. A DPIA is a GDPR obligation; an FRIA is an AI Act obligation. For high-risk AI systems processing personal data, both are required. See [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment).

## Data Processing Agreements and AI Vendors

When an organisation uses a third-party AI provider (e.g., a cloud-based LLM API), the GDPR requires a **Data Processing Agreement** (Article 28) between the data controller (deployer) and the data processor (provider). Key DPA provisions for AI include:

- Restrictions on using customer data for model training
- Data residency requirements
- Sub-processor controls
- Data retention and deletion obligations
- Audit rights

The repository's [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) covers these requirements in detail.

---

**See also:** [DPIA for AI](DPIA-for-AI) · [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI) · [AI Vendor Due Diligence](AI-Vendor-Due-Diligence) · [EU AI Act Overview](EU-AI-Act-Overview) · [Home](Home)

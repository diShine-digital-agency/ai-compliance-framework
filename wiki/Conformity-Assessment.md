# Conformity Assessment

Before a high-risk AI system can be placed on the EU market, the provider must complete a **conformity assessment** to demonstrate that the system meets all requirements of the EU AI Act. This process is governed by Articles 43–49 and detailed in Annexes VI and VII.

## Two Pathways

The AI Act provides two conformity assessment pathways:

### Pathway A: Internal Control (Annex VI)

Self-assessment by the provider, without third-party involvement.

**Applies to:**
- Most standalone high-risk AI systems listed in **Annex III** (employment, education, credit scoring, law enforcement, migration, justice)
- Exception: biometric identification systems (see Pathway B)

**Process:**
1. Verify the quality management system (QMS) is in place and complies with Article 17
2. Examine the technical documentation (Annex IV) to confirm the system meets all requirements (Articles 9–15)
3. Verify that the design and development process is consistent with the documentation
4. Draw up the EU Declaration of Conformity (Article 47)
5. Affix the CE marking (Article 48)
6. Register in the EU AI Database (Article 49)

### Pathway B: Third-Party Assessment via Notified Body (Annex VII)

Independent assessment by an accredited Notified Body.

**Applies to:**
- High-risk AI systems that are **safety components** of products covered by **Annex I** harmonisation legislation (medical devices, machinery, civil aviation, etc.) — the system must go through the conformity assessment procedure of the relevant sectoral legislation
- **Biometric identification systems** used for law enforcement (Annex III, Point 1)

**Process:**
1. The provider applies to a Notified Body
2. The Notified Body examines the provider's QMS (Article 17) and the technical documentation (Annex IV)
3. Assessment of system design, development, and testing
4. Verification of compliance with Articles 9–15
5. The Notified Body issues a certificate (valid for a maximum of 5 years, subject to periodic audits)
6. The provider draws up the EU Declaration of Conformity and affixes the CE marking
7. Registration in the EU AI Database

## Quality Management System (Article 17)

Both pathways require the provider to have a documented QMS that includes:

- A strategy for regulatory compliance
- Techniques, procedures, and systematic actions for design, development, quality control, and quality assurance
- Techniques and procedures for data management (collection, analysis, labelling, storage, filtration, mining, aggregation, retention, and any other operation related to data)
- Design and development of the AI system
- Testing and validation procedures
- Technical specifications, including standards applied
- Systems and procedures for risk management (Article 9)
- Post-market monitoring (Article 72)
- Procedures for reporting serious incidents (Article 73)
- Communication with national authorities, Notified Bodies, and deployers
- Handling and storage of documentation

## Technical Documentation (Annex IV)

The technical documentation must include:

1. **General description** — name, version, intended purpose, provider contact information, intended users
2. **Detailed description** of system elements and development process
3. **Monitoring, functioning, and control** — capabilities, limitations, accuracy levels, foreseeable unintended outcomes and sources of risk
4. **Risk management** — description of the risk management system
5. **Data governance** — training methodologies, data preparation, relevant design choices, origin of datasets, scope and main characteristics of datasets, data labelling
6. **Lifecycle changes** — description of modifications throughout the system's lifecycle
7. **Applied standards** — list of harmonised standards or other means used to demonstrate compliance
8. **Performance metrics** — accuracy, robustness, cybersecurity test results

## CE Marking

Once conformity is established, the provider affixes the **CE marking** to the AI system (or its packaging or documentation). The CE marking indicates that the system conforms to the requirements of the Act and is permitted for market placement in the EU.

For high-risk AI systems, the CE marking must be accompanied by the identification number of the Notified Body (where applicable).

## EU Declaration of Conformity (Article 47)

The provider must draw up a written EU Declaration of Conformity for each high-risk AI system, containing:
- AI system name, type, and unique identification
- Name and address of the provider (and authorised representative, if applicable)
- A statement that the declaration is issued under the sole responsibility of the provider
- Reference to the conformity assessment procedure followed
- Reference to harmonised standards or other specifications applied
- Name and identification number of the Notified Body (if applicable)
- Date of issue and signature

The Declaration must be kept for 10 years after the AI system is placed on the market.

## Notified Bodies (Article 28)

Notified Bodies are independent organisations accredited by **notifying authorities** in each Member State to perform third-party conformity assessments. Requirements include:

- Legal and organisational independence from AI system providers
- Technical competence in AI (staff with knowledge and experience in AI technologies, data, computing, AI risk management, harmonised standards, and relevant Union law)
- Impartiality and absence of conflicts of interest
- Professional liability insurance
- Compliance with confidentiality requirements

## Substantial Modifications

If a high-risk AI system undergoes a **substantial modification** after market placement, a new conformity assessment is required (Article 43(4)). A substantial modification is defined as a change that affects the system's compliance with the requirements of the Act or modifies the intended purpose.

## Relationship to Sector-Specific Legislation

For AI systems that are safety components of products covered by Annex I legislation:
- The AI Act requirements are integrated into the **existing conformity assessment** procedure of the relevant sectoral legislation
- The same Notified Body may assess compliance with both the sectoral legislation and the AI Act
- The provider must ensure compliance with both sets of requirements

This is particularly relevant for medical devices (see [Sector Guide: Healthcare](Sector-Guide-Healthcare)), financial services (see [Sector Guide: Financial Services](Sector-Guide-Financial-Services)), and technology products (see [Sector Guide: Technology](Sector-Guide-Technology)).

## Framework Template

The repository's [Conformity Assessment Pathway Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md) provides a practical walkthrough of both pathways, including a decision flowchart and QMS requirements.

---

**See also:** [High-Risk AI Systems](High-Risk-AI-Systems) · [EU AI Database Registration](EU-AI-Database-Registration) · [EU AI Act Roles](EU-AI-Act-Roles) · [Harmonised Standards (CEN/CENELEC)](Harmonised-Standards) · [Post-Market Monitoring](Post-Market-Monitoring) · [Home](Home)

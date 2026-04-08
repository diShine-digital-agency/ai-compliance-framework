# Sector Guide: Public Administration and Government

Public bodies deploying AI systems face **enhanced obligations** under the EU AI Act. Several Annex III high-risk categories target government functions directly, and public-sector deployers have specific FRIA, transparency, and registration obligations that go beyond those of private entities.

## High-Risk AI Use Cases in Government

| Use Case | Annex III Classification | Risk Level |
|---|---|---|
| **Social benefit eligibility** | 5(a) — Access to essential public services | High-risk |
| **Social benefit calculation/reduction** | 5(a) — Access to essential public services | High-risk |
| **Credit scoring (public banks/agencies)** | 5(b) — Creditworthiness assessment | High-risk |
| **Emergency service dispatching** | 2 — Critical infrastructure | High-risk |
| **Border control and immigration** | 7 — Migration, asylum, border control | High-risk |
| **Asylum application assessment** | 7(c) — Examining applications for asylum | High-risk |
| **Law enforcement — predictive policing** | 6 — Law enforcement | High-risk |
| **Law enforcement — evidence analysis** | 6(b) — Evaluation of evidence reliability | High-risk |
| **Criminal risk assessment** | 6(d) — Profiling of natural persons for crime detection | High-risk |
| **Judicial decision support** | 8 — Administration of justice | High-risk |
| **Biometric identification** | 1 — Biometric identification and categorisation | High-risk (some uses prohibited) |
| **Internal administrative tools** (scheduling, email classification) | Not Annex III | Minimal risk |
| **Public-facing chatbots** | Article 50 transparency | Limited risk |

## Enhanced Obligations for Public Bodies

### 1. Mandatory FRIA with Public Disclosure

Under Article 27, deployers of high-risk AI systems that are **bodies governed by public law** must:
- Conduct a **Fundamental Rights Impact Assessment** before deploying the system
- **Make the FRIA results publicly available** (unlike private-sector deployers, who only submit results to the market surveillance authority)

This creates a significant transparency obligation — the public can scrutinise how government agencies have assessed the fundamental rights impact of their AI systems.

### 2. EU AI Database Registration (Deployer)

Under Article 49, **deployers** of high-risk AI systems that are public bodies must register their use in the **EU AI Database**. This is in addition to the provider's registration obligation.

Private-sector deployers are also required to register in certain cases, but the obligation for public bodies is explicit and comprehensive.

### 3. Article 22 — Right to Explanation

When government AI systems make decisions that affect citizens' rights (benefit eligibility, immigration status, risk assessment), citizens have strong rights under:

- **GDPR Article 22** — right not to be subject to solely automated decisions with legal or similarly significant effects; right to human intervention, right to contest
- **EU Charter Article 41** — right to good administration, including the right to have affairs handled impartially, fairly, and within a reasonable time
- **EU Charter Article 47** — right to an effective remedy and fair trial

Government agencies must ensure that citizens can:
- Receive a **meaningful explanation** of how the AI system contributed to the decision
- **Contest the decision** through an accessible process
- Obtain **human review** by a qualified official
- Access an **effective remedy** if the decision was wrong

### 4. Prohibition on Social Scoring

Article 5(1)(c) explicitly prohibits AI systems used by public authorities for **social scoring** — evaluating or classifying natural persons based on their social behaviour or personal characteristics, where the resulting score leads to detrimental treatment.

This prohibition is absolute for public authorities and applies without exception.

### 5. Biometric Identification Restrictions

Real-time remote biometric identification (RRBIS) in publicly accessible spaces by law enforcement is **prohibited** under Article 5(1)(h), with only three narrow exceptions:
- Targeted search for victims of abduction, trafficking, or sexual exploitation
- Prevention of a specific, substantial, and imminent threat to life or a foreseeable terrorist attack
- Identification of a suspect in a serious criminal offence (as defined in Article 5(2))

Even where exceptions apply:
- Prior judicial or independent administrative authorisation is required
- Each use must be individually assessed for necessity and proportionality
- Temporal, geographic, and personal scope limitations apply

## Good Administration Principles for AI

The EU Charter's right to good administration (Article 41) has specific implications for AI in government:

| Principle | AI Application |
|---|---|
| **Impartiality** | AI systems must not discriminate; bias testing is mandatory |
| **Fairness** | Decisions must be proportionate to their impact on the citizen |
| **Timeliness** | AI should not create unreasonable delays in processing |
| **Right to be heard** | Citizens must have the opportunity to present their case before an adverse decision |
| **Duty to give reasons** | Decisions must be explained; "the AI decided" is not sufficient |
| **Right to access files** | Citizens have the right to access their own case files, including AI-generated assessments |

## Data Governance for Government AI

### Legal Basis for Processing

Government agencies typically rely on these GDPR lawful bases for AI:
- **Article 6(1)(c)** — legal obligation (the AI system is required by law)
- **Article 6(1)(e)** — task carried out in the public interest or in the exercise of official authority

Consent (Article 6(1)(a)) is generally **not appropriate** as a lawful basis for government processing because of the inherent power imbalance between the state and the citizen (EDPB guidance).

### Special Category Data

Government AI systems frequently process special category data:
- Biometric data (border control, identity verification)
- Health data (social services, disability assessments)
- Racial/ethnic origin (migration and asylum systems — creating acute discrimination risks)
- Political opinions, religious beliefs (asylum applications)

Processing of special category data requires both a lawful basis under Article 6 and an exception under Article 9 (typically Article 9(2)(g) — substantial public interest).

### Interoperability and Data Sharing

Government agencies increasingly share data across departments and across Member States. AI systems using shared government data must ensure:
- Data quality — source data may vary in quality across agencies
- Purpose limitation — data collected for one purpose may not be suitable for AI training in another context
- Data protection safeguards — data sharing agreements must address AI-specific risks

## Procurement of AI by Government

When government agencies procure AI from private-sector vendors, they must:

1. **Assess risk classification** — determine whether the procured AI is high-risk
2. **Require conformity assessment documentation** — vendors must provide evidence of compliance
3. **Negotiate deployer obligations** — the procurement contract must address FRIA obligations, transparency requirements, bias testing, and human oversight
4. **Apply the Vendor Audit Checklist** — the [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) is directly applicable to government procurement
5. **DPIA and FRIA** — the government agency (as deployer) is responsible for conducting these assessments, even if the vendor provides a ready-made system

## Framework Templates

| Need | Template |
|---|---|
| FRIA for public-sector deployers | [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) |
| DPIA for government AI | [DPIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) |
| Vendor assessment for government procurement | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) |
| Bias testing | [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) |
| AI literacy for public servants | [AI Literacy Programme](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-literacy-programme.md) |
| Incident response (including regulatory notification) | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |

---

**See also:** [High-Risk AI Systems](High-Risk-AI-Systems) · [Prohibited AI Practices](Prohibited-AI-Practices) · [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment) · [GDPR and AI](GDPR-and-AI) · [EU AI Database Registration](EU-AI-Database-Registration) · [National Implementation by Member States](National-Implementation) · [Home](Home)

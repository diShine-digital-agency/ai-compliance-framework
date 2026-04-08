# Fundamental Rights Impact Assessment (FRIA) for High-Risk AI Systems

**Version:** 2.1.0
**Regulatory Basis:** EU AI Act Article 27, EU Charter of Fundamental Rights

This template implements the **Fundamental Rights Impact Assessment** required by Article 27 of the EU AI Act for deployers of high-risk AI systems. The FRIA is **distinct from and complementary to** a GDPR Data Protection Impact Assessment (DPIA) — it assesses the broader impact on fundamental rights protected by the EU Charter, not only data protection.

**When is a FRIA mandatory?**
*   Deployers of high-risk AI systems listed in Annex III must conduct a FRIA **before** putting the system into use.
*   Bodies governed by public law, or private entities providing public services, must always conduct one.
*   The FRIA must be completed *in addition to* a GDPR DPIA (use the [`dpia-ai-template.md`](dpia-ai-template.md) for the DPIA).

---

## Part 1: System Identification

| Field | Details |
| :--- | :--- |
| **Organisation Name** | [Insert] |
| **AI System Name** | [Insert] |
| **AI System Provider** | [Insert vendor name, if third-party] |
| **Annex III Category** | [e.g., Point 4a — Recruitment & Selection of Employees] |
| **Intended Purpose** | [Describe what the system does and how it will be used] |
| **Deployer Role** | [Public body / Private entity providing public services / Other] |
| **Assessment Date** | [Date] |
| **Assessment Lead** | [Name / Title] |

---

## Part 2: Fundamental Rights Assessment

For each right below, assess whether the AI system poses a risk of interference. If yes, describe the specific risk and the mitigation measures implemented.

### 2.1 Human Dignity (Article 1, EU Charter)
*   **Risk:** Does the system reduce individuals to data points in a way that undermines their inherent dignity? (e.g., algorithmic scoring that dehumanises applicants, automated profiling that creates social hierarchies).
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures, e.g., mandatory human review of all consequential decisions]

### 2.2 Non-Discrimination (Article 21, EU Charter)
*   **Risk:** Does the system risk directly or indirectly discriminating against individuals based on sex, race, colour, ethnic or social origin, genetic features, language, religion, political opinion, membership of a national minority, property, birth, disability, age, or sexual orientation?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures, e.g., algorithmic bias audit conducted per the [Bias Audit Methodology](../guides/algorithmic-bias-audit-methodology.md)]

### 2.3 Right to an Effective Remedy and Fair Trial (Article 47, EU Charter)
*   **Risk:** Can individuals affected by the AI system's decisions effectively challenge them? Is there a clear process for contestation and appeal?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures, e.g., documented contestation procedure, right to human review]

### 2.4 Freedom of Expression and Information (Article 11, EU Charter)
*   **Risk:** Does the system filter, moderate, or rank content in a way that may suppress lawful expression or limit access to information?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures]

### 2.5 Right to Privacy and Data Protection (Articles 7 & 8, EU Charter)
*   **Risk:** Does the system process personal data beyond what is strictly necessary? Does it enable surveillance or tracking?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures. *Note: Detailed data protection risks should be assessed in the separate [DPIA](dpia-ai-template.md).*]

### 2.6 Right to Good Administration (Article 41, EU Charter)
*Applicable primarily to public-sector deployers.*
*   **Risk:** Does the system affect individuals' right to have their affairs handled impartially, fairly, and within a reasonable time?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures]

### 2.7 Workers' Rights (Articles 27–31, EU Charter)
*Applicable when AI is used in employment contexts.*
*   **Risk:** Does the system affect the right to information and consultation (Art. 27), the right to fair and just working conditions (Art. 31), or collective bargaining rights (Art. 28)?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures, e.g., Works Council consulted prior to deployment as per [HR Addendum](sector-addendum-hr.md)]

### 2.8 Rights of the Child (Article 24, EU Charter)
*   **Risk:** Does the system process data of or make decisions about children? Are their best interests considered?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures]

### 2.9 Rights of Persons with Disabilities (Article 26, EU Charter)
*   **Risk:** Does the system's design or outputs create barriers for persons with disabilities? Does it risk discriminating against them?
*   **Assessment:** [No risk identified / Risk identified — describe]
*   **Mitigation:** [Describe measures, e.g., accessibility testing, reasonable accommodation in algorithmic design]

---

## Part 3: Affected Persons & Scale

*   **Categories of persons affected:** [e.g., job applicants, patients, citizens, students]
*   **Estimated number of affected persons:** [Per year / per deployment cycle]
*   **Geographic scope:** [e.g., EU-wide, specific Member State(s)]
*   **Vulnerable populations:** [Are any affected groups considered particularly vulnerable? If yes, describe additional safeguards.]

---

## Part 4: Specific Risks to Groups (Article 27(1)(c))

*   **Identified groups at particular risk:** [Based on the Art. 21 protected characteristics and the system's specific domain — e.g., in a recruitment AI, women in STEM fields; in a credit scoring AI, ethnic minorities in specific geographic areas.]
*   **Measures for affected groups:** [Specific mitigation for each identified group.]

---

## Part 5: Human Oversight & Contestation

*   **Human oversight mechanism:** [Describe how human oversight is implemented per AI Act Article 14 — e.g., human-in-the-loop, human-on-the-loop, or human-in-command]
*   **Contestation mechanism:** [How can an affected person contest a decision? What is the timeline for response?]
*   **Escalation path:** [If the deployer cannot resolve, what is the path to the national Market Surveillance Authority?]

---

## Part 6: Notification & Record-Keeping

*   **FRIA results notification:** Under Article 27(4), the results of this FRIA must be submitted to the relevant national **Market Surveillance Authority (MSA)** as part of the registration process (see the [EU AI Database Registration Guide](eu-ai-database-registration-guide.md)).
*   **Record retention:** This FRIA must be retained for the entire duration of the AI system's deployment and for at least **10 years** after the system is decommissioned.

---

## Part 7: Sign-Off

| Role | Name | Signature | Date |
| :--- | :--- | :--- | :--- |
| **Assessment Lead** | [Name] | _______________ | [Date] |
| **Legal Counsel** | [Name] | _______________ | [Date] |
| **DPO** | [Name] | _______________ | [Date] |
| **Senior Management** | [Name] | _______________ | [Date] |

---
*This template is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 3 — Architect & Deploy**, **Step 3.5: Conduct the Fundamental Rights Impact Assessment**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

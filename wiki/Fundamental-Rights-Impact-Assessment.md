# Fundamental Rights Impact Assessment (FRIA)

The Fundamental Rights Impact Assessment is a distinct obligation under **EU AI Act Article 27**. It requires deployers of high-risk AI systems to assess the impact of the system on fundamental rights enshrined in the EU Charter of Fundamental Rights before putting the system into service.

The FRIA is **separate from and complementary to** the GDPR Data Protection Impact Assessment (DPIA). For high-risk AI systems processing personal data, both assessments are typically required.

## Who Must Conduct an FRIA

Deployers of high-risk AI systems that are:
- **Bodies governed by public law** (government agencies, public authorities)
- **Private entities providing public services** (healthcare, education, utilities)
- **Deployers of high-risk AI systems** listed in certain Annex III categories (credit scoring, insurance pricing, essential service eligibility)

## When to Conduct an FRIA

The FRIA must be completed **before** the high-risk AI system is put into service. It should be updated:
- When the AI system is substantially modified
- When the context of use changes materially
- When new risks are identified through post-deployment monitoring

## Rights Assessed

The FRIA assesses the impact on nine categories of fundamental rights from the EU Charter:

| EU Charter Article | Right | AI Relevance |
|---|---|---|
| **Article 1** | Human dignity | AI systems must not undermine the inherent worth and dignity of individuals |
| **Article 21** | Non-discrimination | AI systems must not discriminate on grounds of sex, race, colour, ethnic or social origin, genetic features, language, religion, political opinion, membership of a national minority, property, birth, disability, age, or sexual orientation |
| **Articles 7–8** | Privacy and data protection | AI systems processing personal data must respect privacy rights and data protection principles |
| **Article 11** | Freedom of expression and information | AI systems must not unduly restrict freedom of expression or access to information |
| **Article 47** | Right to an effective remedy and fair trial | Persons affected by AI decisions must have access to effective legal remedies |
| **Article 41** | Right to good administration | AI systems used in public administration must ensure fair, timely, and transparent decision-making |
| **Articles 27–31** | Workers' rights | AI systems in the workplace must respect the right to fair working conditions, information and consultation, protection against unjustified dismissal, and collective bargaining |
| **Article 24** | Rights of the child | AI systems affecting children must prioritise the child's best interests |
| **Article 26** | Rights of persons with disabilities | AI systems must ensure integration and accessibility for persons with disabilities |

## FRIA Process

### Step 1: System Description
- Identify the high-risk AI system
- Describe the intended purpose and context of use
- Identify the affected population
- Describe the deployment environment

### Step 2: Stakeholder Engagement
- Identify relevant stakeholders (affected persons, workers, civil society)
- Consult with stakeholders where appropriate
- Document consultation outcomes

### Step 3: Rights Impact Analysis
For each of the nine rights categories:
- Assess whether the AI system may have a positive, negative, or neutral impact
- Describe the nature and severity of any negative impact
- Identify affected groups, particularly vulnerable populations
- Assess the likelihood and severity of harm

### Step 4: Mitigation Measures
For each identified negative impact:
- Describe technical measures (bias mitigation, explainability, human oversight)
- Describe organisational measures (training, governance, complaint mechanisms)
- Assess residual risk after mitigation

### Step 5: Documentation and Sign-Off
- Document the complete assessment
- Obtain sign-off from the responsible officer
- Submit results to the EU AI Database as part of the registration process (Article 49)

### Step 6: Notification
- Notify the relevant **market surveillance authority** of the FRIA results
- For public-sector deployers: make the FRIA publicly available

## Relationship to DPIA

| Aspect | DPIA | FRIA |
|---|---|---|
| **Legal instrument** | GDPR | EU AI Act |
| **Scope of rights** | Privacy and data protection | All EU Charter fundamental rights |
| **Trigger** | High risk to data subjects from personal data processing | Deployment of high-risk AI system |
| **Conducted by** | Data controller (DPO) | Deployer of AI system |
| **Submitted to** | National DPA (if prior consultation needed) | Market surveillance authority + EU AI Database |
| **Recurrence** | When processing changes | When system or context changes |

**In practice:** Many organisations conduct both assessments in parallel, with the FRIA expanding the scope of the risk analysis beyond data protection to cover all fundamental rights. The DPIA focuses on personal data risks (bias, automated decisions, data leakage); the FRIA adds non-discrimination, workers' rights, children's rights, dignity, and access to justice.

## Framework Template

The repository's [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) provides a structured format for conducting the assessment, including:
- System description section
- All nine rights categories with assessment prompts
- Mitigation measures documentation
- Sign-off workflow
- MSA notification guidance

---

**See also:** [DPIA for AI](DPIA-for-AI) · [High-Risk AI Systems](High-Risk-AI-Systems) · [EU AI Database Registration](EU-AI-Database-Registration) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [Home](Home)

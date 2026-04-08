# High-Risk AI Systems

High-risk AI systems are at the core of the EU AI Act's regulatory framework. They are permitted on the EU market but subject to the Act's most demanding compliance requirements. The high-risk obligations take full effect on **2 August 2026**.

## What Makes an AI System High-Risk

An AI system is classified as high-risk through one of two routes:

### Route 1: Safety Components of Regulated Products (Article 6(1))

An AI system is high-risk if it is intended to be used as a **safety component** of a product (or is itself a product) covered by the EU harmonisation legislation listed in **Annex I**, and the product is required to undergo a third-party conformity assessment.

Annex I legislation includes:
- Medical Devices Regulation (MDR 2017/745)
- In Vitro Diagnostic Medical Devices Regulation (IVDR 2017/746)
- Machinery Regulation (EU) 2023/1230
- Toys Safety Directive
- Radio Equipment Directive
- Lifts Directive
- Civil Aviation Safety (Regulation (EC) 216/2008)
- Motor Vehicles and Trailers type-approval
- Rail Systems Safety
- Marine Equipment

### Route 2: Standalone High-Risk Use Cases (Article 6(2), Annex III)

AI systems in specific use-case categories listed in **Annex III** are high-risk:

| Category | Annex III Ref. | Examples |
|----------|---------------|----------|
| **Biometrics** | 1 | Remote biometric identification (non-real-time), biometric categorisation (outside Article 5 prohibitions) |
| **Critical infrastructure** | 2 | Safety components managing road traffic, water supply, gas, heating, electricity |
| **Education and vocational training** | 3 | Systems determining access to education, assessing learning outcomes, detecting prohibited behaviour during exams |
| **Employment, workers management, and access to self-employment** | 4(a), 4(b) | Recruitment and selection (CV parsing, video interview analysis), promotion and termination decisions, task allocation, performance monitoring |
| **Access to and enjoyment of essential private and public services and benefits** | 5(a)–5(c) | Creditworthiness assessment, insurance risk and pricing, eligibility for public benefits, emergency service dispatch prioritisation |
| **Law enforcement** | 6 | Polygraphs, assessing the reliability of evidence, profiling in criminal investigations, crime analytics |
| **Migration, asylum, and border control management** | 7 | Risk assessments for irregular migration, examination of visa and asylum applications, verification of travel documents |
| **Administration of justice and democratic processes** | 8 | AI assisting judicial authorities in researching and interpreting law, applying the law to facts |

### The Filtering Mechanism (Article 6(3))

An Annex III AI system is **not** considered high-risk if it does not pose a **significant risk of harm** to health, safety, or fundamental rights. Specifically, a system is not high-risk if it:

- Performs a narrow procedural task
- Improves the result of a previously completed human activity
- Detects decision-making patterns or deviations from prior patterns without replacing or influencing human assessment
- Performs only a preparatory task to an assessment relevant to the purposes listed in Annex III

The provider must **document the rationale** for applying this filtering mechanism and make it available to the national authority on request.

## Requirements for High-Risk AI Systems

Providers of high-risk AI systems must comply with the following requirements:

### 1. Risk Management System (Article 9)

A continuous, iterative process throughout the AI system's lifecycle:
- Identification and analysis of known and foreseeable risks
- Estimation and evaluation of risks that may emerge under conditions of reasonably foreseeable misuse
- Adoption of appropriate risk management measures
- Testing procedures to ensure risks are effectively mitigated

### 2. Data and Data Governance (Article 10)

Training, validation, and testing datasets must be subject to appropriate data governance, including:
- Relevant design choices
- Data collection processes and origin
- Data preparation operations (annotation, labelling, cleaning, enrichment)
- Formulation of relevant assumptions regarding information the data is supposed to measure
- Assessment of the availability, quantity, and suitability of the datasets needed
- Examination of possible biases
- Identification of data gaps or shortcomings and how they can be addressed

### 3. Technical Documentation (Article 11, Annex IV)

Comprehensive documentation drawn up before the system is placed on the market, including:
- General description of the AI system
- Detailed description of system elements and development process
- Information about monitoring, functioning, and control
- Description of the risk management system
- Description of changes throughout the lifecycle
- A list of applied harmonised standards or other means of compliance
- Accuracy, robustness, and cybersecurity metrics

### 4. Record-Keeping (Article 12)

High-risk AI systems must include automatic recording of events (logs) throughout their lifetime:
- Recording of the period of each use
- The reference database against which input data was checked
- Input data for which the search led to a match
- Identification of natural persons involved in the verification of results

### 5. Transparency and Provision of Information to Deployers (Article 13)

High-risk AI systems must be designed to allow deployers to interpret and use the system's output appropriately:
- Clear instructions of use
- Characteristics, capabilities, and limitations
- Intended purpose and foreseeable misuse scenarios
- Human oversight measures
- Expected lifetime, maintenance, and update arrangements

### 6. Human Oversight (Article 14)

Systems must be designed to allow effective oversight by natural persons:
- Oversight must enable understanding of the system's capacities and limitations
- Persons must be able to correctly interpret output
- Persons must be able to decide not to use the system or to override its output
- Persons must be able to intervene or interrupt the system

### 7. Accuracy, Robustness, and Cybersecurity (Article 15)

Systems must achieve appropriate levels of:
- **Accuracy** — declared in the instructions of use
- **Robustness** — resilient to errors, faults, and inconsistencies, including adversarial manipulation (adversarial robustness)
- **Cybersecurity** — protected against attempts to alter use or performance by exploiting vulnerabilities

## Conformity Assessment

Before placing a high-risk AI system on the market, the provider must complete a conformity assessment:

- **Pathway A (Internal Control):** Self-assessment under Annex VI for most standalone Annex III systems
- **Pathway B (Notified Body):** Third-party assessment under Annex VII for systems that are safety components of products regulated under Annex I legislation, and for biometric identification systems

See [Conformity Assessment](Conformity-Assessment) for the full process.

## Post-Market Obligations

After market placement, providers must:
- Implement a **post-market monitoring system** (Article 72)
- Report **serious incidents** to the relevant market surveillance authority within **15 days** (Article 73)
- Cooperate with market surveillance authorities (Article 74)

## Deployer Obligations

Deployers of high-risk AI systems have their own set of obligations (see [EU AI Act Roles](EU-AI-Act-Roles)):
- Use the system in accordance with instructions
- Assign qualified human oversight
- Monitor system operation
- Conduct a [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment) (Article 27) before deployment in certain cases
- Retain system logs for at least six months
- Inform affected natural persons

## Framework Templates for High-Risk Systems

| Obligation | Framework Template |
|---|---|
| Overall compliance journey | [Step-by-Step User Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/how-to-use-this-framework.md) |
| Vendor assessment | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) |
| Conformity assessment | [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md) |
| DPIA | [DPIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) |
| FRIA | [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) |
| Bias audit | [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) |
| Database registration | [EU AI Database Registration Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/eu-ai-database-registration-guide.md) |
| Incident response | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |
| Sector-specific rules | [Sector Addenda](Repository-Guide) (Finance, Healthcare, HR, Technology, Beauty) |

---

**See also:** [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification) · [Conformity Assessment](Conformity-Assessment) · [EU AI Act Roles](EU-AI-Act-Roles) · [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment) · [Home](Home)

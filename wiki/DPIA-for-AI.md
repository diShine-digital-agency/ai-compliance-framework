# DPIA for AI

A Data Protection Impact Assessment (DPIA) is a structured process for identifying and mitigating risks to individuals arising from personal data processing. For AI systems, a DPIA is a **mandatory prerequisite** under GDPR Article 35 when the processing is likely to result in a high risk to the rights and freedoms of natural persons.

## When Is a DPIA Required

A DPIA is **mandatory** for AI systems in these situations:

1. **Systematic and extensive evaluation of personal aspects** — profiling, scoring, or automated decision-making that produces legal or similarly significant effects (directly matches most AI use cases)
2. **Processing of special category data on a large scale** — health data, biometric data, racial/ethnic origin, etc.
3. **Systematic monitoring of publicly accessible areas** — CCTV with AI analytics, crowd monitoring
4. **New technologies** — the European Data Protection Board (EDPB) has confirmed that AI/ML qualifies as a "new technology" triggering the DPIA obligation

National data protection authorities have published **blacklists** of processing operations that always require a DPIA. AI-based profiling, automated decision-making, and large-scale processing of special category data appear on most national lists.

## DPIA vs. FRIA

| | DPIA | FRIA |
|---|---|---|
| **Legal basis** | GDPR Article 35 | EU AI Act Article 27 |
| **Focus** | Personal data protection risks | Fundamental rights impact (broader than data protection) |
| **Scope** | Any processing likely to result in high risk to individuals | High-risk AI systems deployed in certain categories |
| **Who conducts** | Data controller (typically the DPO) | Deployer of the high-risk AI system |
| **When** | Before processing begins | Before the AI system is put into service |
| **Relationship** | Complementary — both may be required for the same system |

For high-risk AI systems processing personal data, **both** a DPIA and an FRIA are typically required. The DPIA addresses data protection risks; the FRIA addresses broader fundamental rights impacts (dignity, non-discrimination, freedom of expression, etc.). See [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment).

## AI-Specific Risks to Assess

Standard DPIAs may not adequately address AI-specific risks. The repository's DPIA template adds four AI-specific risk categories:

### 1. Algorithmic Bias
AI models can encode and amplify biases present in training data, leading to discriminatory outcomes. Assess:
- Protected characteristics that may be affected
- Whether training data is representative
- Whether proxy variables could introduce indirect discrimination
- What bias testing has been conducted

### 2. Opacity and Explainability
Many AI models (particularly deep learning) operate as "black boxes." Assess:
- Whether the model's decision logic can be explained to data subjects
- Whether meaningful information about the logic involved can be provided (GDPR Recital 71)
- What explainability techniques are available (LIME, SHAP, counterfactual explanations)

### 3. Automated Decision-Making
If the AI system makes or informs decisions that produce legal or similarly significant effects:
- Does the processing fall under GDPR Article 22?
- Is there a valid exception (contract, law, explicit consent)?
- Are the Article 22 safeguards in place (human intervention, right to contest)?

### 4. Data Leakage and Model Inversion
AI models can memorise and regurgitate training data, and adversarial techniques (model inversion, membership inference) can extract information about individuals in the training set. Assess:
- Whether the model retains personal data from training
- What privacy-preserving techniques are applied (differential privacy, federated learning)
- Whether the model is exposed to adversarial attack vectors

## DPIA Process

1. **Describe the processing** — system description, purpose, data flows, data categories, retention periods
2. **Assess necessity and proportionality** — is the processing necessary for the stated purpose? Could a less intrusive approach achieve the same result?
3. **Identify and assess risks** — systematic evaluation of risks to individuals, including AI-specific risks
4. **Identify mitigation measures** — technical and organisational measures to reduce risks
5. **Document residual risk** — after mitigation, what risk remains?
6. **Obtain DPO opinion** — the DPO must provide advice on the DPIA
7. **Prior consultation (if needed)** — if residual risk remains high despite mitigation, the data controller must consult the national data protection authority under GDPR Article 36 **before** processing begins

## Prior Consultation Triggers

If, after applying all mitigation measures, the residual risk to individuals remains **high**, the organisation must submit the DPIA to the national data protection authority for **prior consultation** under GDPR Article 36. The authority has 8 weeks (extendable to 14 weeks) to respond.

Failure to conduct a required DPIA or to consult when required can result in GDPR fines of up to €10 million / 2% of turnover.

## Framework Templates

| Resource | Link |
|---|---|
| AI-specific DPIA template | [DPIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) |
| Three pre-filled DPIA examples | [DPIA Example Library](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-example-library.md) |
| Bias assessment methodology | [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) |

The DPIA Example Library includes three complete examples:
1. **AI Recruitment Screening Tool** — algorithmic bias risks, Article 22 obligations, mandatory human oversight
2. **AI Customer Service Chatbot with Sentiment Analysis** — special category data inference, DLP masking, Article 50 transparency
3. **AI Employee Performance Monitoring** — profiling risks, Works Council consultation, mandatory prior SA consultation trigger

---

**See also:** [GDPR and AI](GDPR-and-AI) · [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [Home](Home)

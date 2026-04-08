# Sector Guide: Human Resources

Employment and worker management is explicitly listed in **Annex III, Points 4(a) and 4(b)** of the EU AI Act as a high-risk domain. AI systems used in recruitment, performance evaluation, task allocation, and workforce management are subject to the full suite of high-risk requirements.

## High-Risk AI Use Cases in HR

| Use Case | Annex III Classification | Risk Level |
|---|---|---|
| **CV screening / parsing** | 4(a) — Recruitment and selection | High-risk |
| **Video interview analysis** | 4(a) — Recruitment and selection | High-risk |
| **Automated shortlisting** | 4(a) — Recruitment and selection | High-risk |
| **Performance monitoring** | 4(b) — Decisions affecting terms of work | High-risk |
| **Promotion/termination decisions** | 4(b) — Decisions affecting terms of work | High-risk |
| **Task allocation** | 4(b) — Decisions affecting terms of work | High-risk |
| **Emotion recognition in interviews** | Article 5(1)(f) — **Prohibited** | Banned |
| **Emotion recognition in workplace** | Article 5(1)(f) — **Prohibited** | Banned |
| **Training recommendation** | Generally not Annex III | Minimal risk |
| **Scheduling optimisation** | Generally not Annex III | Minimal risk |

## Key Regulatory Requirements

### 1. Human Oversight — Meaningful, Not Rubber-Stamping

Article 14 requires human oversight that is **effective and meaningful**. For HR AI:

- A human reviewer must have the authority, competence, and time to override AI recommendations
- Simply confirming AI-generated shortlists without genuine review is insufficient ("rubber-stamping")
- The human must have access to the AI system's reasoning and relevant information about the candidate
- Override rates should be monitored — if humans never override the AI, the oversight may be ineffective

### 2. GDPR Article 22 — Automated Decision-Making

Most HR AI use cases fall within Article 22 because they:
- Are based **solely** (or substantially) on automated processing
- Produce **legal effects** (hiring, termination) or **similarly significantly affect** the individual

When Article 22 applies:
- The data subject has the right **not to be subject to the decision** (unless an exception applies)
- The data controller must implement **safeguards**: right to human intervention, right to express their point of view, right to contest the decision
- The data subject must be provided with **meaningful information about the logic involved**

### 3. Transparency to Workers (Article 26)

Deployers of high-risk AI in the workplace must:
- Inform **workers' representatives** and the affected **workers** that they will be subject to a high-risk AI system **before** putting the system into service
- In many Member States, this triggers **Works Council consultation** obligations under national labour law

### 4. Prohibition on Workplace Emotion Recognition

Article 5(1)(f) **prohibits** AI systems that infer the emotions of employees in the workplace, except for medical or safety purposes. This means:

- ❌ Monitoring employees' facial expressions during meetings to assess engagement
- ❌ Analysing voice tone in customer service calls to evaluate employee performance
- ❌ Using sentiment analysis in video interviews for recruitment
- ✅ Detecting driver drowsiness for road safety (medical/safety exception)
- ✅ Monitoring stress indicators in safety-critical roles (medical/safety exception)

### 5. Bias Testing

HR AI is particularly susceptible to bias because:
- Historical hiring data often reflects historical discrimination
- Name, address, education institution, and language can serve as proxies for protected characteristics
- Interview analysis systems may exhibit bias based on accent, appearance, or communication style

The [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) should be applied to all HR AI systems. At minimum:
- Disparate impact testing across gender, age, ethnicity, and disability
- Regular monitoring of selection rates by protected group
- Documentation of the fairness criteria chosen and the justification for that choice

## Works Council and Employee Consultation

Many EU Member States have specific laws requiring **Works Council consultation** before deploying AI systems that affect workers:

| Country | Requirement |
|---|---|
| **Germany** | Works Constitution Act (BetrVG) §87 — co-determination rights for monitoring equipment and AI in personnel planning |
| **France** | Labour Code — obligation to consult the Social and Economic Committee (CSE) before introducing surveillance or performance monitoring technology |
| **Netherlands** | Works Councils Act — consent required for monitoring systems |
| **Belgium** | CBA No. 39 — rules on electronic surveillance |

Non-compliance with Works Council obligations can render the AI deployment unlawful under national labour law, independently of the AI Act.

## Framework Template

The repository's [Human Resources & Employment Sector Addendum](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-hr.md) covers:
- Annex III Point 4 classification guidance
- Mandatory human oversight design (non-rubber-stamping)
- GDPR Article 22 implementation
- Bias mitigation for recruitment AI
- Works Council consultation requirements by country
- Transparency obligations to workers

The [DPIA Example Library](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-example-library.md) includes two HR-relevant DPIA examples:
1. **AI Recruitment Screening Tool** — algorithmic bias, Article 22 obligations
2. **AI Employee Performance Monitoring** — profiling risks, Works Council consultation

---

**See also:** [High-Risk AI Systems](High-Risk-AI-Systems) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [Prohibited AI Practices](Prohibited-AI-Practices) · [GDPR and AI](GDPR-and-AI) · [DPIA for AI](DPIA-for-AI) · [Home](Home)

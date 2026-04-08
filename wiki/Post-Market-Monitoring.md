# Post-Market Monitoring (Article 72)

Post-market monitoring is a **proactive, continuous obligation** on providers of AI systems to systematically monitor their systems after market placement or putting into service. It is distinct from incident response — post-market monitoring is ongoing and preventive; incident response is reactive and triggered by a specific event.

For providers of **high-risk AI systems**, post-market monitoring is a mandatory component of the quality management system (Article 17) and must be documented in a formal post-market monitoring plan.

## Legal Basis

| Provision | Scope |
|---|---|
| **Article 72** | Post-market monitoring obligations for all AI system providers |
| **Article 72(3)** | Enhanced post-market monitoring plan for high-risk AI system providers |
| **Article 9** | Risk management system — post-market monitoring feeds into the continuous risk management process |
| **Article 17** | Quality management system — post-market monitoring is a required component |
| **Article 73** | Serious incident reporting — triggered when post-market monitoring detects a serious incident |
| **Article 20** | Corrective actions — when monitoring identifies non-compliance or risk |

## Post-Market Monitoring vs. Incident Response

| Aspect | Post-Market Monitoring | Incident Response |
|---|---|---|
| **Nature** | Proactive, continuous, systematic | Reactive, event-triggered |
| **Purpose** | Detect emerging risks before they cause harm; verify ongoing compliance | Contain and mitigate harm from a specific incident |
| **Timing** | Ongoing throughout the AI system's lifecycle | When a specific incident occurs |
| **Legal basis** | Article 72 | Article 73 (reporting) + organisational IRP |
| **Output** | Monitoring data, trend analysis, risk updates | Incident report, regulatory notification, corrective action |
| **Relationship** | Monitoring may detect an incident, triggering the response process | Incident response may identify monitoring gaps, improving the monitoring programme |

## What Must Be Monitored

The post-market monitoring system should systematically collect, document, and analyse data relevant to:

### 1. Performance Monitoring

- **Accuracy** — does the system continue to perform as intended? Are key performance metrics (precision, recall, F1, AUC) stable?
- **Robustness** — does the system perform reliably under varying conditions, including edge cases and adversarial inputs?
- **Consistency** — are outputs consistent over time, or is there evidence of instability?

### 2. Fairness and Bias Monitoring

- **Bias drift** — are fairness metrics (demographic parity, equal opportunity, equalized odds) stable over time, or are disparities emerging or widening?
- **Group-level performance** — does the system perform equally well for all population groups, including those defined by protected characteristics?
- **Feedback loops** — is the system creating or amplifying biases through its influence on future data?

See [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) for the statistical framework.

### 3. Data Quality and Drift

- **Data drift** — has the distribution of input data changed since the system was trained or last validated? Feature distributions, data volume patterns, and input quality should be monitored.
- **Concept drift** — has the relationship between inputs and the correct output changed? (e.g., consumer behaviour changes that make a recommendation model less effective)
- **Data quality degradation** — are there new sources of missing, corrupted, or biased data entering the system?

### 4. User Feedback and Complaints

- **User reports** — systematic collection of user feedback, complaints, and error reports
- **Human oversight observations** — feedback from human overseers about system behaviour, including cases where humans override or disagree with the AI
- **Downstream impact** — information from deployers about how the system is performing in their specific context

### 5. Security and Adversarial Monitoring

- **Adversarial attacks** — monitoring for prompt injection attempts, adversarial inputs, or attempts to manipulate system behaviour
- **Model integrity** — verifying that model weights and configurations have not been tampered with
- **Vulnerability monitoring** — tracking disclosed vulnerabilities in AI components, libraries, and frameworks

### 6. Regulatory and Environmental Changes

- **New guidance** — Commission guidelines, harmonised standards, or enforcement decisions that affect compliance
- **Context changes** — changes in the deployment environment that could affect system risk (new user populations, new use cases by deployers)
- **Legal developments** — new legislation, court decisions, or regulatory interpretations

## The Post-Market Monitoring Plan

For **high-risk AI systems**, Article 72(3) requires a documented post-market monitoring plan that must:

1. **Define monitoring activities** — what data is collected, what metrics are tracked, and how they are analysed
2. **Establish monitoring frequency** — how often each type of data is reviewed (continuous, daily, weekly, quarterly)
3. **Specify thresholds and triggers** — define performance thresholds that trigger investigation, corrective action, or incident reporting
4. **Assign responsibilities** — identify who is responsible for each monitoring activity
5. **Document escalation procedures** — how findings are escalated, including triggers for:
   - Updating the risk management system (Article 9)
   - Reporting a serious incident (Article 73)
   - Initiating corrective action (Article 20)
   - Updating technical documentation (Article 11)
   - Conducting a new conformity assessment (if a substantial modification has occurred)
6. **Record retention** — maintain monitoring data and analysis for the AI system's expected lifespan plus 10 years (per Article 18)

## Serious Incident Reporting (Article 73)

When post-market monitoring (or any other mechanism) identifies a **serious incident**, the provider must report it to the relevant national market surveillance authority within **15 days** of becoming aware.

A **serious incident** is defined as an incident or malfunctioning that directly or indirectly leads to:
- Death or serious damage to health
- Serious damage to property or the environment
- A serious and irreversible disruption of the management and operation of critical infrastructure
- A serious breach of fundamental rights obligations

The serious incident report must include:
- Description of the AI system and the incident
- Corrective measures taken or planned
- Impact assessment (who was affected, how, and to what extent)

See [AI Incident Response](AI-Incident-Response) for the full incident response framework.

## When Is a New Conformity Assessment Required?

Post-market monitoring may reveal that a **substantial modification** to the AI system is needed. Under Article 43(4), a new conformity assessment is required when:

- The AI system undergoes a **substantial modification** — a change that is not foreseen by the provider in the original conformity assessment and that may affect compliance with the AI Act requirements
- The **intended purpose** of the AI system changes

If the corrective action resulting from monitoring constitutes a substantial modification, the provider must conduct a new conformity assessment before placing the modified system on the market.

## Practical Implementation

### Monitoring Architecture

| Layer | Tools and Techniques |
|---|---|
| **Data monitoring** | Data drift detectors, input validation, schema checks, missing data alerts |
| **Model monitoring** | Performance dashboards, fairness metric tracking, prediction distribution analysis |
| **System monitoring** | Uptime, latency, error rates, resource utilisation |
| **User feedback** | Complaint management systems, human oversight logs, deployer feedback channels |
| **Security monitoring** | Adversarial input detection, log analysis, model integrity checks |

### Integration with Risk Management

Post-market monitoring data must feed into the risk management system required by Article 9. This creates a continuous improvement cycle:

1. **Monitor** — collect post-market data on performance, fairness, and incidents
2. **Analyse** — identify trends, anomalies, and emerging risks
3. **Update risk assessment** — revise the risk management system with new findings
4. **Implement corrective action** — address identified risks through system updates, additional safeguards, or operational changes
5. **Document** — update technical documentation to reflect changes
6. **Report** — notify the market surveillance authority of serious incidents and material changes

## Framework Templates

| Need | Template |
|---|---|
| Risk management integration | [ISO 42001 Alignment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/iso42001-alignment-guide.md) |
| Incident detection and response | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |
| Bias monitoring methodology | [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) |
| Vendor monitoring | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) |
| Conformity assessment (re-assessment triggers) | [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md) |

---

**See also:** [High-Risk AI Systems](High-Risk-AI-Systems) · [AI Incident Response](AI-Incident-Response) · [Conformity Assessment](Conformity-Assessment) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [ISO 42001 and AI Governance Standards](ISO-42001-and-AI-Governance-Standards) · [Home](Home)

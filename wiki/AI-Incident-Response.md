# AI Incident Response

AI systems introduce incident categories that traditional IT incident response frameworks do not adequately address. The EU AI Act (Article 73) requires providers of high-risk AI systems to report **serious incidents** to the relevant market surveillance authority. The GDPR (Articles 33–34) imposes separate breach notification obligations when personal data is involved.

## What Constitutes an AI Incident

AI incidents extend beyond data breaches to include:

| Category | Examples |
|---|---|
| **Prompt injection** | Adversarial inputs that bypass safety filters, extract system prompts, or cause unintended behaviour |
| **Model inversion / data extraction** | Attacks that extract training data or personal information from a model |
| **Algorithmic bias discovery** | Discovery that a deployed model produces discriminatory outcomes |
| **Hallucination with real-world impact** | Model generates false information (fake citations, fabricated facts) that is acted upon |
| **Unintended output** | Model produces harmful, offensive, or legally problematic content |
| **Model drift** | Model performance degrades over time, leading to inaccurate or unfair outcomes |
| **Data poisoning** | Training data is deliberately corrupted to influence model behaviour |
| **Shadow AI exposure** | Employees leak confidential data through unauthorised AI tools |

## Regulatory Notification Requirements

| Regulation | Trigger | Deadline | Report To |
|---|---|---|---|
| **EU AI Act (Art. 73)** | Serious incident involving high-risk AI | **15 days** after becoming aware | National market surveillance authority |
| **GDPR (Art. 33)** | Personal data breach | **72 hours** after becoming aware | National Data Protection Authority |
| **GDPR (Art. 34)** | High-risk personal data breach | Without undue delay | Affected data subjects |
| **NIS2** | Significant cybersecurity incident | **24 hours** initial; **72 hours** detailed | National CSIRT |
| **DORA** | Major ICT-related incident (financial sector) | **4 hours** initial | National financial supervisor |

A single AI incident may trigger notification obligations under multiple regimes simultaneously.

## Severity Taxonomy

The repository's [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) uses a P1–P4 severity taxonomy:

| Priority | Description | Response Time | Notification |
|---|---|---|---|
| **P1 — Critical** | Confirmed bias causing harm; large-scale data extraction; regulatory violation | Immediate | CEO, DPO, Legal, Regulator |
| **P2 — High** | Prompt injection with data exposure; model producing harmful outputs in production | Within 4 hours | CISO, DPO, Legal |
| **P3 — Medium** | Model drift exceeding thresholds; minor bias identified in testing | Within 24 hours | AI Governance Lead |
| **P4 — Low** | Shadow AI usage detected; minor hallucination without impact | Within 72 hours | IT Director |

## The Six-Phase Response Framework

### Phase 1: Preparation
- Establish an AI-specific incident response team with defined roles
- Develop response procedures for each AI incident category
- Conduct tabletop exercises with AI-specific scenarios
- Implement monitoring and alerting for AI system behaviour
- Maintain forensic preservation capabilities for model weights and logs

### Phase 2: Detection and Identification
- Monitor model performance metrics for anomalies
- Implement adversarial testing and red-teaming programmes
- Monitor user reports and feedback channels
- Track bias metrics in production
- Monitor for prompt injection patterns

### Phase 3: Containment
- Determine whether the AI system should be:
  - **Isolated** (remove from production while preserving for forensics)
  - **Rate-limited** (reduce access while investigating)
  - **Modified** (apply safety filters or rollback to a previous version)
  - **Shut down** (in cases of confirmed serious harm)
- Preserve model weights, logs, and input/output data for forensic analysis
- Prevent further harm to affected individuals

### Phase 4: Forensic Investigation
- Analyse root cause:
  - Was the issue in training data, model architecture, deployment configuration, or adversarial input?
  - Was it a known vulnerability or a novel attack?
- Document the chain of events with timestamps
- Preserve evidence for regulatory reporting and potential litigation
- Assess the scope of impact (how many individuals affected, what data was exposed, what decisions were influenced)

### Phase 5: Regulatory Notification
- Determine which notification obligations are triggered (AI Act, GDPR, NIS2, DORA)
- Prepare notification content per each regime's requirements
- Submit notifications within the required timelines
- Communicate with affected individuals where required
- Coordinate with legal counsel on liability implications

### Phase 6: Recovery and Lessons Learned
- Implement corrective measures (model retraining, data governance improvements, additional safeguards)
- Update the risk management system (Article 9)
- Update technical documentation (Article 11)
- Conduct a post-incident review
- Update the incident response playbook based on lessons learned
- Consider whether a new conformity assessment is required (if a substantial modification was made)

## Framework Template

The repository's [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) provides a comprehensive, ready-to-use playbook aligned with:
- EU AI Act Article 73 (Serious Incident Reporting)
- GDPR Articles 33/34 (Breach Notification)
- ENISA AI Threat Landscape
- NIST AI RMF 1.0

---

**See also:** [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI) · [Shadow AI: Risks and Mitigation](Shadow-AI) · [High-Risk AI Systems](High-Risk-AI-Systems) · [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines) · [Home](Home)

# ISO 42001 and AI Governance Standards

ISO/IEC 42001:2023 is the first international standard for an **Artificial Intelligence Management System (AIMS)**. Published in December 2023, it provides a framework for organisations to establish, implement, maintain, and continually improve their management of AI throughout its lifecycle.

## What Is ISO/IEC 42001

ISO 42001 follows the same **Annex SL** high-level structure used by ISO 9001 (quality), ISO 27001 (information security), and ISO 14001 (environmental management). This makes it compatible with existing management systems and enables integrated management.

It consists of:
- **10 core clauses** defining the management system requirements
- **Annex A** with 39 controls specific to AI governance
- **Annex B** providing implementation guidance for those controls
- **Annex C** mapping to other relevant standards (ISO 27001, ISO 27701, ISO 23894)
- **Annex D** guidance on AI-specific objectives and risk sources

## Core Clauses

| Clause | Topic | Key Requirements |
|---|---|---|
| 4 | Context of the Organisation | Understanding internal/external issues; interested parties; scope of the AIMS |
| 5 | Leadership | Management commitment; AI policy; roles and responsibilities |
| 6 | Planning | Risk assessment and treatment; AI objectives; planned changes |
| 7 | Support | Resources; competence; awareness; communication; documented information |
| 8 | Operation | Operational planning and control; AI risk assessment; AI risk treatment; AI system impact assessment |
| 9 | Performance Evaluation | Monitoring, measurement, analysis, evaluation; internal audit; management review |
| 10 | Improvement | Nonconformity and corrective action; continual improvement |

## Annex A Controls (Selected)

| Control Area | Examples |
|---|---|
| **AI Policy** | Establish an AI policy aligned with organisational objectives |
| **AI System Lifecycle** | Controls for each phase: design, development, verification, validation, deployment, operation, retirement |
| **Data for AI Systems** | Data quality, provenance, preparation, annotation, bias assessment |
| **AI System Impact** | Impact assessment considering individuals, groups, and society |
| **AI System Documentation** | Technical documentation for development, operations, and users |
| **Third-Party Relationships** | Supply chain governance for AI components |
| **AI System Monitoring** | Continuous monitoring of AI system performance, fairness, and safety |
| **Logging and Auditability** | Logging of AI system decisions and events for audit purposes |

## Relationship to the EU AI Act

### Does ISO 42001 Certification Create Presumption of Conformity?

**Not automatically.** Article 40 of the EU AI Act establishes that high-risk AI systems that conform to **harmonised European standards** are presumed to comply with the corresponding AI Act requirements. However:

1. ISO 42001 is an **international standard** (ISO/IEC), not a **harmonised European standard** (CEN/CENELEC).
2. CEN and CENELEC are developing European standards for AI that are expected to reference or build upon ISO 42001, but these have not yet been finalised.
3. Once harmonised European standards are adopted that incorporate ISO 42001 principles, compliance with those standards will create a presumption of conformity.

### Practical Value

Despite not creating a direct presumption of conformity, ISO 42001 certification provides:

- **Evidence of "state-of-the-art" governance** — demonstrates to regulators, customers, and partners that the organisation follows international best practices
- **Structured foundation** — the AIMS provides the governance structure needed to comply with AI Act requirements
- **Audit readiness** — the management system's documentation, internal audit, and management review processes prepare the organisation for regulatory inspections
- **Competitive advantage** — in procurement, ISO 42001 certification signals compliance maturity

### Mapping ISO 42001 to AI Act Requirements

| AI Act Requirement | ISO 42001 Alignment |
|---|---|
| Risk management (Art. 9) | Clause 6 (Planning — risk assessment), Annex A (AI system impact assessment) |
| Data governance (Art. 10) | Annex A (Data for AI systems) |
| Technical documentation (Art. 11) | Clause 7 (Documented information), Annex A (Documentation) |
| Human oversight (Art. 14) | Annex A (Human oversight controls) |
| Accuracy, robustness, cybersecurity (Art. 15) | Clause 8 (Operational controls), Annex A (Monitoring) |
| Post-market monitoring (Art. 72) | Clause 9 (Performance evaluation), Annex A (Monitoring) |
| Quality management system (Art. 17) | Clauses 4–10 (the entire AIMS) |

## The 12-Month Implementation Roadmap

The repository's [ISO/IEC 42001 Alignment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/iso42001-alignment-guide.md) provides a practical 12-month roadmap for mid-market enterprises:

### Phase 1 — Foundation (Months 1–3)
- Gap assessment against ISO 42001 requirements
- Define AIMS scope
- Establish AI governance committee
- Draft AI policy
- AI risk assessment

### Phase 2 — Design & Documentation (Months 4–6)
- Develop the statement of applicability (select applicable Annex A controls)
- Design processes for the AI system lifecycle
- Establish data governance procedures
- Define impact assessment methodology
- Document all procedures and policies

### Phase 3 — Implementation (Months 7–9)
- Implement selected controls
- Deploy monitoring and logging
- Conduct AI literacy training (aligns with Article 4)
- Perform impact assessments for existing AI systems
- Establish supply chain governance for AI vendors

### Phase 4 — Audit & Certification (Months 10–12)
- Conduct internal audits
- Management review
- Address nonconformities
- Stage 1 certification audit (document review)
- Stage 2 certification audit (implementation verification)

## Other Relevant Standards

| Standard | Focus |
|---|---|
| **ISO/IEC 23894:2023** | AI risk management guidance |
| **ISO/IEC 38507:2022** | Governance of IT — governance implications of the use of AI |
| **ISO/IEC 27001:2022** | Information security management (complements ISO 42001 for cybersecurity aspects) |
| **ISO/IEC 27701:2019** | Privacy information management (extends ISO 27001 for GDPR compliance) |
| **ISO/IEC 25059:2023** | AI systems quality model |
| **NIST AI RMF 1.0** | US-based AI risk management framework (complementary, not a substitute for EU requirements) |

## Europrivacy / GDPR Certification

In addition to ISO 42001, organisations may seek **Europrivacy certification** (the first official GDPR certification scheme under Article 42). While focused on data protection rather than AI governance specifically, it provides accredited evidence of GDPR compliance that complements the AIMS.

---

**See also:** [EU AI Act Overview](EU-AI-Act-Overview) · [Conformity Assessment](Conformity-Assessment) · [High-Risk AI Systems](High-Risk-AI-Systems) · [AI Literacy Obligation](AI-Literacy-Obligation) · [Home](Home)

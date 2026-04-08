# Sector Guide: Financial Services

Financial services is one of the sectors most heavily affected by the EU AI Act due to the classification of several common AI applications as high-risk under Annex III, combined with existing sector-specific regulation (DORA, MiFID II, Solvency II).

## High-Risk AI Use Cases in Finance

| Use Case | Annex III Classification | Risk Level |
|---|---|---|
| **Credit scoring** | 5(b) — Access to essential services | High-risk |
| **Insurance risk and pricing** | 5(b) — Access to essential services | High-risk |
| **Loan approval** | 5(b) — Access to essential services | High-risk |
| **Benefit eligibility** | 5(a) — Access to essential services | High-risk |
| **Robo-advisory** | Potentially 5(c) depending on impact | Case-by-case |
| **Fraud detection** | Generally not Annex III (security purpose) | Typically limited/minimal risk |
| **Customer chatbots** | Not Annex III (but Article 50 transparency) | Limited risk |
| **Internal analytics** | Not Annex III | Minimal risk |

## Regulatory Convergence

Financial institutions using AI face a **triple regulatory burden**:

### 1. EU AI Act
- High-risk system requirements (Articles 9–15) for credit scoring, insurance pricing, and loan approval
- Conformity assessment, EU AI Database registration, FRIA
- Article 50 transparency for customer-facing AI (chatbots)

### 2. DORA (Digital Operational Resilience Act)
- **ICT risk management** covering AI-based services
- **Incident reporting** — major ICT-related incidents must be reported within 4 hours (initial) to national financial supervisors
- **Third-party risk management** — AI vendors are ICT third-party service providers under DORA
- **Digital operational resilience testing** — includes AI systems

### 3. GDPR Article 22
- Automated decision-making in credit and insurance decisions triggers Article 22
- Right not to be subject to solely automated decisions with legal/significant effects
- Right to human intervention, to express a point of view, and to contest the decision
- Must provide "meaningful information about the logic involved"

### 4. MiFID II (for investment-related AI)
- **Suitability assessment** — AI-driven investment advice must demonstrate suitability for the individual client
- **Best execution** — algorithmic trading must comply with best execution obligations
- **Record-keeping** — all algorithmic trading decisions must be recorded and retained

## Bias Risks in Financial AI

Credit scoring and insurance pricing AI carry acute bias risks:

- **Historical discrimination** — models trained on historical lending data may perpetuate past discriminatory practices (e.g., redlining)
- **Proxy discrimination** — variables like postcode, occupation, or purchase history may serve as proxies for protected characteristics
- **Disparate impact** — even facially neutral models may produce disproportionate rejection rates for protected groups

The [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) provides the statistical framework for testing these risks.

## Practical Compliance Steps

1. **Classify** all AI systems used in financial operations against Annex III
2. **Conduct DPIAs** for all systems processing personal data for credit, insurance, or benefit decisions
3. **Implement Article 22 safeguards** — human review mechanisms, contestation procedures
4. **Audit for bias** — regular disparate impact testing across protected characteristics
5. **Align DORA and AI Act incident reporting** — harmonise internal procedures to meet both timelines
6. **Vendor due diligence** — assess AI vendors against both DORA ICT third-party requirements and AI Act vendor audit criteria

## Framework Template

The repository's [Financial Services Sector Addendum](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-finance.md) maps these requirements in detail, including DORA integration and MiFID II explainability requirements.

---

**See also:** [High-Risk AI Systems](High-Risk-AI-Systems) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI) · [GDPR and AI](GDPR-and-AI) · [Home](Home)

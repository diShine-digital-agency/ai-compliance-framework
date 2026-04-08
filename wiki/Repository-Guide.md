# Repository Guide

This page provides a complete map of every file in the [AI Compliance Framework repository](https://github.com/diShine-digital-agency/ai-compliance-framework), with descriptions, target audience, and links.

## Recommended Reading Order

The framework is designed to be used in a specific sequence. The [Step-by-Step User Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/how-to-use-this-framework.md) maps the full journey across four phases:

1. **Phase 1 — Assess & Contain** (Days 1–14): Quantify Shadow AI exposure, establish policies
2. **Phase 2 — Audit & Procure** (Days 15–45): Vet vendors, apply sector-specific rules
3. **Phase 3 — Architect & Deploy** (Days 45–90): Choose deployment tiers, conduct assessments, register systems
4. **Phase 4 — Monitor & Respond** (Ongoing): Incident response, continuous governance

## Directory Structure

```
ai-compliance-framework/
├── README.md                           # Project overview and navigation
├── CONTRIBUTING.md                     # How to contribute
├── SECURITY.md                         # Security policy
├── CHANGELOG.md                        # Version history
├── LICENSE                             # MIT License
├── .github/
│   └── workflows/
│       └── sync-wiki.yml               # Auto-syncs wiki/ to GitHub Wiki
├── assets/                             # Images, diagrams
├── guides/                             # Strategic guides
│   ├── how-to-use-this-framework.md
│   ├── algorithmic-bias-audit-methodology.md
│   └── ai-liability-product-safety.md
├── templates/                          # Actionable templates
│   ├── acceptable-use-policy.md
│   ├── ai-incident-response-playbook.md
│   ├── ai-literacy-programme.md
│   ├── conformity-assessment-guide.md
│   ├── deployment-decision-matrix.md
│   ├── dpia-ai-template.md
│   ├── dpia-example-library.md
│   ├── eu-ai-database-registration-guide.md
│   ├── fria-template.md
│   ├── gpai-model-governance-checklist.md
│   ├── iso42001-alignment-guide.md
│   ├── prompt-ip-guidelines.md
│   ├── sector-addendum-beauty.md
│   ├── sector-addendum-finance.md
│   ├── sector-addendum-healthcare.md
│   ├── sector-addendum-hr.md
│   ├── sector-addendum-tech.md
│   ├── shadow-ai-risk-calculator.md
│   └── vendor-audit-checklist.md
├── tools/                              # Interactive tools
│   └── compliance-toolkit.html
└── wiki/                               # Wiki source files (auto-synced to GitHub Wiki)
    ├── Home.md                         # Wiki landing page
    ├── About-This-Framework.md
    ├── Repository-Guide.md
    ├── FAQ.md
    ├── Glossary.md
    ├── Key-Regulatory-References.md
    ├── EU-AI-Act-Overview.md
    ├── EU-AI-Act-Risk-Classification.md
    ├── EU-AI-Act-Enforcement-Timeline.md
    ├── EU-AI-Act-Penalties-and-Fines.md
    ├── EU-AI-Act-Roles.md
    ├── Prohibited-AI-Practices.md
    ├── High-Risk-AI-Systems.md
    ├── General-Purpose-AI-GPAI.md
    ├── Transparency-Obligations.md
    ├── Conformity-Assessment.md
    ├── EU-AI-Database-Registration.md
    ├── Post-Market-Monitoring.md
    ├── GDPR-and-AI.md
    ├── EU-Regulatory-Landscape-for-AI.md
    ├── AI-Liability-in-the-EU.md
    ├── National-Implementation.md
    ├── Regulatory-Sandboxes.md
    ├── Harmonised-Standards.md
    ├── Open-Source-AI-and-the-EU-AI-Act.md
    ├── DPIA-for-AI.md
    ├── Fundamental-Rights-Impact-Assessment.md
    ├── Shadow-AI.md
    ├── AI-Vendor-Due-Diligence.md
    ├── Algorithmic-Bias-and-Fairness.md
    ├── AI-Incident-Response.md
    ├── AI-Literacy-Obligation.md
    ├── IP-Protection-and-AI.md
    ├── ISO-42001-and-AI-Governance-Standards.md
    ├── AI-Governance-and-Board-Oversight.md
    ├── Sector-Guide-Financial-Services.md
    ├── Sector-Guide-Healthcare.md
    ├── Sector-Guide-Human-Resources.md
    ├── Sector-Guide-Technology.md
    ├── Sector-Guide-Beauty-and-Cosmetics.md
    ├── Sector-Guide-Education.md
    └── Sector-Guide-Public-Administration.md
```

## File-by-File Reference

### Guides

| File | Description | Primary Audience |
|------|-------------|------------------|
| [Step-by-Step User Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/how-to-use-this-framework.md) | Master orchestration guide — maps the full compliance journey across 4 phases, assigns owners to each step, explains the regulatory rationale | All roles |
| [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) | 4-phase statistical audit methodology covering Demographic Parity, Equal Opportunity, Equalized Odds, Predictive Parity, and the Chouldechova/Kleinberg impossibility theorems | Data Scientists, Compliance Officers |
| [AI Liability & Product Safety Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/ai-liability-product-safety.md) | The EU's three-pillar liability framework: AI Act (rules), AI Liability Directive (fault-based), revised Product Liability Directive (strict liability) | Legal Counsel, C-Suite, Risk Management |

### Templates — Policy & Training

| File | Description | Primary Audience |
|------|-------------|------------------|
| [Acceptable AI Use Policy](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/acceptable-use-policy.md) | Customisable corporate policy mapping data classification tiers to approved AI tiers, addressing Shadow AI risks | CISO, Legal, HR, All Employees |
| [AI Literacy Programme](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-literacy-programme.md) | Role-based training framework implementing EU AI Act Article 4, with 4-module curriculum and assessment standards | HR, Legal, All Employees |
| [Prompt Engineering IP Protection](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/prompt-ip-guidelines.md) | 5 techniques for preventing IP leakage through AI prompts, addressing the Trade Secrets Directive | Engineering Leads, All Employees |

### Templates — Assessment & Audit

| File | Description | Primary Audience |
|------|-------------|------------------|
| [Shadow AI Risk Calculator](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/shadow-ai-risk-calculator.md) | 100-point self-assessment across 4 dimensions with risk band mapping and remediation roadmap | CISO, IT Director, C-Suite |
| [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) | 25-point AI-specific vendor due diligence covering GDPR, EU AI Act, and security requirements | Procurement, DPO, Legal |
| [DPIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) | AI-specific Data Protection Impact Assessment for GDPR Article 35 | DPO, Product Owner |
| [DPIA Example Library](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-example-library.md) | 3 pre-filled DPIA examples: AI Recruitment, Chatbot with Sentiment Analysis, Employee Monitoring | DPO, Compliance Officers |
| [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) | EU AI Act Article 27 Fundamental Rights Impact Assessment for deployers of high-risk systems | Legal Counsel, DPO |
| [GPAI Model Governance Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/gpai-model-governance-checklist.md) | Compliance checklist for GPAI models under Articles 53–55, including Code of Practice alignment | AI Engineering Leads, Procurement |

### Templates — Architecture & Registration

| File | Description | Primary Audience |
|------|-------------|------------------|
| [Deployment Decision Matrix](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/deployment-decision-matrix.md) | 4-tier architectural decision framework balancing data sensitivity, cost, and regulatory requirements | CTO, Enterprise Architecture, DPO |
| [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md) | Two pathways: Internal Control (Annex VI) vs. Notified Body (Annex VII) for high-risk AI providers | QA, Legal, AI Providers |
| [EU AI Database Registration](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/eu-ai-database-registration-guide.md) | Step-by-step registration procedure under Article 49 for high-risk systems | Legal, AI Engineering Leads |
| [ISO/IEC 42001 Alignment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/iso42001-alignment-guide.md) | 12-month roadmap for AIMS implementation and ISO 42001 certification preparation | COO, CISO, AI Governance Leads |

### Templates — Incident Management

| File | Description | Primary Audience |
|------|-------------|------------------|
| [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) | 6-phase response framework with P1–P4 severity taxonomy, regulatory notification timelines | CISO, Security Operations, Incident Response |

### Templates — Sector Addenda

| File | Description | Primary Audience |
|------|-------------|------------------|
| [Financial Services](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-finance.md) | DORA, MiFID II, credit scoring, insurance pricing | Compliance Officers (Finance) |
| [Healthcare](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-healthcare.md) | MDR/IVDR, CDSS, triage chatbots, GDPR Article 9 health data | Compliance Officers (Healthcare) |
| [Human Resources](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-hr.md) | Annex III.4 recruitment AI, performance monitoring, Works Council consultation | HR, Legal |
| [Technology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-tech.md) | Provider vs. Deployer roles, NIS2, CRA, SaaS obligations | CTO, Product Managers |
| [Beauty & Cosmetics](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-beauty.md) | Virtual try-on, skin analysis, biometric categorisation, Cosmetics Regulation | Product Managers (Beauty) |

### Tools

| File | Description |
|------|-------------|
| [Interactive Compliance Toolkit](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/tools/compliance-toolkit.html) | Standalone, client-side HTML app with Shadow AI Risk Calculator, Vendor Compliance Scorecard, and Deployment Tier Advisor. Runs entirely in the browser — no data transmitted externally. |

---

**See also:** [About This Framework](About-This-Framework) · [Home](Home)

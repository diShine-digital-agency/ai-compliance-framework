# 🛡️ Enterprise AI Compliance Toolkit: operational guardrails for corporate innovation

<div align="center">
  
[![diShine Logo](https://dishine.it/favicon.ico)](https://dishine.it/)

***Transform. Automate. Shine!***

[![Website](https://img.shields.io/badge/Website-dishine.it-blue)](https://dishine.it/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-diShine-blue)](https://linkedin.com/company/100682596)
[![Location](https://img.shields.io/badge/Location-Milan%2C%20Italy-green)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-lightgrey)](LICENSE)

<p align="center">
  <img src="assets/ai_compliance_05_executive_compliance_workbench.webp" alt="AI Compliance workbench" width="85%">
</p>

*The Enterprise AI Compliance Toolkit is a practical framework for adopting AI responsibly in corporate environments, balancing innovation with regulatory compliance. Built in collaboration with legal advisors, this repository provides templates, decision matrices, and audit checklists for navigating the **EU AI Act**, **GDPR**, and corporate **Intellectual Property (IP)** protection.*

*Updated: April 2026 | Version 2.2.1*

# More details / official wiki on [the website](https://compliance.dishine.it).

> **📚 Looking for more?** Explore the **[AI Compliance Framework Wiki](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki)** for in-depth regulatory deep dives, a glossary, FAQ, sector-specific guides, and step-by-step compliance walkthroughs beyond these templates.

Built by [diShine Digital Agency](https://dishine.it).

</div>

<p align="center">
  <img src="assets/ai_compliance_02_vendor_audit_scorecard.webp" alt="AI Compliance audit scorecard" width="49%">
  <img src="assets/ai_compliance_04_governance_document_report.webp" alt="AI Compliance report" width="49%">
</p>

<p align="center">
  <img src="assets/ai_compliance_03_deployment_tier_advisor.webp" alt="AI Compliance deployment tier advisor" width="60%">
</p>

---

## The Problem: shadow AI and regulatory uncertainty

Enterprise AI adoption faces two systemic risks:
1. **Shadow AI:** Employees using consumer-grade AI tools (ChatGPT, Claude, Gemini) without IT oversight, leading to IP leaks (e.g., the 2023 Samsung source code incident) and potential GDPR violations. Gartner estimates that by 2026, 80% of employees will use generative AI for work without company approval.
2. **Regulatory Uncertainty:** Legal and compliance teams blocking AI initiatives due to the EU AI Act (penalties reach up to €35M or 7% of global turnover for prohibited practices, €15M or 3% for high-risk system violations, and €7.5M or 1% for providing incorrect information) and complex, phased enforcement timelines.

This framework provides the operational guardrails to deploy AI while maintaining data sovereignty and regulatory compliance.

## What's inside

This repository contains ready-to-use Markdown templates and strategic guidelines. **New to the framework? Start with the [Step-by-Step User Guide](guides/how-to-use-this-framework.md)**, it explains the correct sequence for deploying these tools, who should own each step, and why each step matters.

### 0. 📖 [Step-by-Step User Guide](guides/how-to-use-this-framework.md)
A comprehensive guide that walks any team through the full AI compliance journey across four phases: Assess & Contain, Audit & Procure, Architect & Deploy, and Monitor & Respond. Each step references the correct template, names the responsible owner (CISO, DPO, CTO, etc.), and explains the regulatory and business rationale behind the action.

### 1. 📄 [Acceptable AI Use Policy Template](templates/acceptable-use-policy.md)
A customizable corporate policy that defines exactly what employees can and cannot do with AI tools. It categorizes data (Public, Internal, Confidential, Restricted) and maps it to approved AI tiers, explicitly addressing the risks of Shadow AI.

### 2. 🛡️ [AI Vendor Audit Checklist (GDPR & EU AI Act)](templates/vendor-audit-checklist.md)
A rigorous 25-point checklist for evaluating third-party AI vendors. It goes beyond standard security questionnaires to address specific AI risks: model training data provenance, Article 22 (automated decision-making) implications, and EU AI Act GPAI obligations.

### 3. 🏗️ [Enterprise AI Deployment Decision Matrix](templates/deployment-decision-matrix.md)
A strategic framework for CTOs and IT Directors to choose the right architectural tier for any AI project:
- **Tier 1:** Consumer APIs (High Risk)
- **Tier 2:** Enterprise API Agreements (Medium Risk)
- **Tier 3:** Private Cloud / VPC Deployment (Low Risk)
- **Tier 4:** Self-Hosted Open-Source Models (Zero External Risk)

### 4. 🔒 [Prompt Engineering IP Protection Guidelines](templates/prompt-ip-guidelines.md)
Technical and legal guidelines on preventing Intellectual Property leakage through AI prompts. Covers redaction techniques, the legal definition of trade secret disclosure via LLMs, and the critical difference between system prompts and user prompts.

### 5. 🧮 [Shadow AI Risk Calculator](templates/shadow-ai-risk-calculator.md)
A scored self-assessment tool (100 points across 4 sections) that quantifies your organization's current Shadow AI exposure. The result maps to a risk band (Managed / Moderate / Elevated / Critical) with a concrete remediation roadmap. Based on IBM's 2024 Cost of a Data Breach Report and Gartner's Shadow AI research.

### 6. 📊 [Data Protection Impact Assessment (DPIA) for AI](templates/dpia-ai-template.md)
A specialized DPIA template designed specifically for AI systems, addressing algorithmic bias, opacity, and GDPR Article 22 (Automated Decision-Making) requirements.

### 7. 🌐 [ISO/IEC 42001:2023 Alignment Guide](templates/iso42001-alignment-guide.md)
A practical 12-month roadmap for mid-market enterprises to implement an Artificial Intelligence Management System (AIMS) and prepare for ISO 42001 certification.

### 8. 🏢 Sector-Specific Addenda
Industry-specific regulatory mapping and risk classifications:
*   [Financial Services Addendum](templates/sector-addendum-finance.md) (DORA, MiFID II, Credit Scoring)
*   [Technology Sector Addendum](templates/sector-addendum-tech.md) (Provider vs. Deployer, NIS2, CRA)
*   [Beauty & Cosmetics Addendum](templates/sector-addendum-beauty.md) (MDR, Biometric Categorization, EU Cosmetics Regulation)
*   [Healthcare & Life Sciences Addendum](templates/sector-addendum-healthcare.md) (MDR/IVDR, CDSS, GDPR Art. 9 Health Data)
*   [Human Resources & Employment Addendum](templates/sector-addendum-hr.md) (Annex III.4, Art. 22 Automated Decisions, Emotion Recognition Prohibition)

### 9. 📋 [DPIA Example Library](templates/dpia-example-library.md)
Three pre-filled, pragmatic Data Protection Impact Assessment (DPIA) examples for the most common enterprise AI deployments, covering GDPR Article 35 requirements. For the separate EU AI Act Article 27 Fundamental Rights Impact Assessment, see the standalone [FRIA Template](templates/fria-template.md).
*   **AI Recruitment Screening Tool**: algorithmic bias risks, Art. 22 obligations, mandatory human oversight;
*   **AI Customer Service Chatbot with Sentiment Analysis**: special category data inference, DLP masking, Art. 50 transparency;
*   **AI Employee Performance Monitoring**: profiling risks, Works Council consultation, mandatory prior SA consultation trigger.

### 10. 🚨 [AI Incident Response Playbook](templates/ai-incident-response-playbook.md)
A structured, forensic AI incident response framework aligned with EU AI Act Article 73 (Serious Incident Reporting), GDPR Articles 33/34, and the ENISA AI Threat Landscape. Covers the full 6-phase response lifecycle, a P1–P4 severity taxonomy, regulatory notification timelines (15-day AI Act window, 72-hour GDPR window), and specific response tactics for prompt injection, model inversion, and algorithmic bias discovery.

### 11. 🤖 [GPAI Model Governance Checklist](templates/gpai-model-governance-checklist.md)
A practical compliance checklist for organizations that develop, fine-tune, or deploy General Purpose AI (GPAI) models under EU AI Act Articles 53–55. Covers the 10^25 FLOPs systemic risk threshold, Article 53 baseline obligations (technical documentation, Annex XI/XII, copyright policy, training data summary), Article 55 systemic risk obligations (adversarial red-teaming, AI Office incident reporting), deployer due diligence requirements, and the GPAI Code of Practice (published July 2025) as a presumption-of-compliance path.

### 12. ⚖️ [Algorithmic Bias Audit Methodology Guide](guides/algorithmic-bias-audit-methodology.md)
A rigorous, step-by-step methodology for conducting an algorithmic fairness audit, grounded in statistical theory and current EU regulatory requirements. Covers the four core statistical fairness criteria (Demographic Parity, Equal Opportunity, Equalized Odds, Predictive Parity) with exact mathematical definitions; the Chouldechova (2017) and Kleinberg et al. (2016) impossibility theorems and their practical audit implications; a 4-phase audit methodology (pre-audit scoping, data bias audit, model bias audit, intersectional audit); bias mitigation strategies (pre-processing, in-processing, post-processing) with their accuracy-fairness trade-offs; and EU AI Act Article 10 compliance documentation requirements.

### 13. 🛠️ [Interactive Compliance Toolkit](tools/compliance-toolkit.html)
A standalone, client-side web application that brings three key framework components to life as interactive tools:
*   **Shadow AI Risk Calculator**: automated scoring across four dimensions (Organizational Awareness, Technical Controls, Data Governance, Incident History) with risk band determination and remediation recommendations.
*   **Vendor Compliance Scorecard**: interactive 25-item checklist tracking progress against EU AI Act and GDPR vendor requirements, with compliance grading and gap reporting.
*   **Deployment Tier Advisor**: a guided 3-question decision tree that recommends the appropriate deployment architecture (Tier 2–4) based on data sensitivity, infrastructure capability, and regulatory requirements.

No data is transmitted externally, the toolkit runs entirely in the browser.

### 14. 🔍 [Fundamental Rights Impact Assessment (FRIA) Template](templates/fria-template.md)
A standalone FRIA template implementing EU AI Act Article 27, distinct from the GDPR DPIA. Assesses impact on EU Charter fundamental rights including human dignity (Art. 1), non-discrimination (Art. 21), right to effective remedy (Art. 47), freedom of expression (Art. 11), privacy (Arts. 7–8), workers' rights (Arts. 27–31), rights of children (Art. 24), and rights of persons with disabilities (Art. 26). Includes sign-off workflow and MSA notification requirements.

### 15. 🎓 [AI Literacy Programme Template](templates/ai-literacy-programme.md)
A practical template for implementing the EU AI Act Article 4 AI literacy obligation (in force since February 2025). Provides a role-based needs assessment matrix, a four-module core curriculum (AI Fundamentals, Regulatory Landscape, Responsible AI for Technical Teams, Human Oversight in Practice), delivery and assessment standards, and guidance on evidencing compliance to regulators.

### 16. 🗄️ [EU AI Database Registration Guide](templates/eu-ai-database-registration-guide.md)
A step-by-step guide for registering high-risk AI systems in the EU AI Database as required by Article 49. Covers provider and deployer registration obligations, required information per Annex VIII, the registration procedure, and penalties for non-registration (up to €15M / 3% of turnover).

### 17. ✅ [Conformity Assessment Pathway Guide](templates/conformity-assessment-guide.md)
A practical guide for providers of high-risk AI systems to navigate the conformity assessment process. Explains the two pathways: Internal Control (Annex VI) for most Annex III systems vs. Third-Party Assessment via Notified Body (Annex VII) for regulated products and biometric identification. Includes a decision flowchart, QMS requirements (Article 17), technical documentation requirements (Annex IV), and CE marking procedures.

### 18. ⚖️ [AI Liability & Product Safety Guide](guides/ai-liability-product-safety.md)
A comprehensive guide to the EU's three-pillar liability framework for AI: the EU AI Act (rules), the AI Liability Directive (fault-based liability with presumption of causality), and the revised Product Liability Directive 2024/2853 (strict liability extending to software and AI). Covers the transposition deadline (December 2026), burden of proof lightening, post-deployment learning liability, and practical implications for both providers and deployers.

# Complementary wiki on [the website](https://compliance.dishine.it).

## Visual reference

### Enterprise AI Deployment Tiers
![Enterprise AI Deployment Tiers](assets/deployment-tiers.png)

### EU AI Act Enforcement Timeline
![EU AI Act Enforcement Timeline](assets/eu-ai-act-timeline.png)

---

## How to use this framework

For a full walkthrough of every step, see the **[Step-by-Step User Guide](guides/how-to-use-this-framework.md)**. It covers the correct sequence, the responsible owner for each action, and the regulatory rationale behind every tool in this repository.

In brief: start with the [Interactive Compliance Toolkit](tools/compliance-toolkit.html) or the [Shadow AI Risk Calculator](templates/shadow-ai-risk-calculator.md) to quantify your current exposure, then establish the rules with the [Acceptable AI Use Policy](templates/acceptable-use-policy.md) and [AI Literacy Programme](templates/ai-literacy-programme.md), audit your existing vendors with the [Vendor Audit Checklist](templates/vendor-audit-checklist.md), and use the [Deployment Decision Matrix](templates/deployment-decision-matrix.md) to govern every new AI initiative. The sector-specific addenda, DPIA/[FRIA](templates/fria-template.md) templates, [Conformity Assessment Guide](templates/conformity-assessment-guide.md), and audit methodology guides apply when you are deploying high-risk AI systems.

## 📚 Wiki: in-depth knowledge base

For background knowledge, regulatory deep dives, and reference material beyond these templates, see the **[AI Compliance Framework Wiki](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki)**.

The wiki covers:
- **EU AI Act**: [overview](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/EU-AI-Act-Overview), [risk classification](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/EU-AI-Act-Risk-Classification), [enforcement timeline](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/EU-AI-Act-Enforcement-Timeline), [penalties](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/EU-AI-Act-Penalties-and-Fines), [roles](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/EU-AI-Act-Roles), [prohibited practices](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Prohibited-AI-Practices), [high-risk systems](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/High-Risk-AI-Systems), [GPAI](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/General-Purpose-AI-GPAI), [transparency obligations](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Transparency-Obligations), [post-market monitoring](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Post-Market-Monitoring)
- **Related regulations**: [GDPR & AI](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/GDPR-and-AI), [regulatory landscape](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/EU-Regulatory-Landscape-for-AI) (NIS2, DORA, CRA, DSA, PLD), [AI liability](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/AI-Liability-in-the-EU), [national implementation](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/National-Implementation), [regulatory sandboxes](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Regulatory-Sandboxes), [harmonised standards](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Harmonised-Standards), [open-source AI](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Open-Source-AI-and-the-EU-AI-Act)
- **Compliance processes**: [DPIA](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/DPIA-for-AI), [FRIA](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Fundamental-Rights-Impact-Assessment), [vendor due diligence](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/AI-Vendor-Due-Diligence), [bias auditing](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Algorithmic-Bias-and-Fairness), [incident response](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/AI-Incident-Response), [Shadow AI](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Shadow-AI)
- **Governance**: [board oversight](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/AI-Governance-and-Board-Oversight), [ISO 42001](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/ISO-42001-and-AI-Governance-Standards), [AI literacy](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/AI-Literacy-Obligation)
- **Sector guides**: [financial services](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Financial-Services), [healthcare](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Healthcare), [HR](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Human-Resources), [technology](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Technology), [beauty & cosmetics](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Beauty-and-Cosmetics), [education](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Education), [public administration](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Sector-Guide-Public-Administration)
- **Reference**: [glossary](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Glossary), [key regulatory references](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/Key-Regulatory-References), [FAQ](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki/FAQ)

The wiki is automatically synced from the [`wiki/`](wiki/) directory in this repository via GitHub Actions.

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md) for guidelines on how to contribute to this framework.

## Security

See [SECURITY.md](SECURITY.md) for the security policy and vulnerability reporting process.

## About diShine

[diShine](https://dishine.it) is a creative tech agency based in Milan. We create digital strategies, design process and build tools for clients, help businesses with AI strategy and MarTech architecture, and open-source some things we wish existed.

- Web: [dishine.it](https://dishine.it)
- GitHub: [github.com/diShine-digital-agency](https://github.com/diShine-digital-agency)
- Contact: kevin@dishine.it

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. You are free to use, modify, and distribute these templates within your organization.

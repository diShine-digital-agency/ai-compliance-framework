# AI Compliance Framework for Enterprises

A pragmatic, business-first framework for adopting AI safely in corporate environments without stifling innovation. 

Built by [diShine Digital Agency](https://dishine.it), this repository provides the templates, decision matrices, and audit checklists to help mid-market and enterprise clients navigate the intersection of the **EU AI Act**, **GDPR**, and corporate **Intellectual Property (IP)** protection. Produced in collaboration with a legal advisor team.

*Updated: April 2026 — Version 1.4.1*

---

## The Problem: Shadow AI and Regulatory Paralysis

Enterprise AI adoption is currently trapped between two extremes:
1. **Shadow AI:** Employees using consumer-grade tools (like ChatGPT Plus or Claude Pro) without IT oversight, leading to documented IP leaks (e.g., the 2023 Samsung source code incident) and GDPR violations. Gartner estimates that by 2026, 80% of employees will use generative AI for work without company approval.
2. **Regulatory Paralysis:** Legal and compliance teams blocking all AI initiatives due to fear of the EU AI Act (with fines up to €35M or 7% of global turnover) and GDPR enforcement.

**This framework bridges the gap.** It provides the operational guardrails necessary to deploy AI rapidly while maintaining strict data sovereignty and regulatory compliance.

## What's Inside

This repository contains ready-to-use Markdown templates and strategic guidelines. **New to the framework? Start with the [Step-by-Step User Guide](guides/how-to-use-this-framework.md)** — it explains the correct sequence for deploying these tools, who should own each step, and why each step matters.

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
Three pre-filled, pragmatic Data Protection Impact Assessment (DPIA) examples for the most common enterprise AI deployments, combining GDPR Article 35 and EU AI Act Article 30 (Fundamental Rights Impact Assessment) requirements:
*   **AI Recruitment Screening Tool** — algorithmic bias risks, Art. 22 obligations, mandatory human oversight;
*   **AI Customer Service Chatbot with Sentiment Analysis** — special category data inference, DLP masking, Art. 50 transparency;
*   **AI Employee Performance Monitoring** — profiling risks, Works Council consultation, mandatory prior SA consultation trigger.

### 10. 🚨 [AI Incident Response Playbook](templates/ai-incident-response-playbook.md)
A structured, forensic AI incident response framework aligned with EU AI Act Article 73 (Serious Incident Reporting), GDPR Articles 33/34, and the NIST AI RMF 1.0. Covers the full 6-phase response lifecycle, a P1–P4 severity taxonomy, regulatory notification timelines (15-day AI Act window, 72-hour GDPR window), and specific response tactics for prompt injection, model inversion, and algorithmic bias discovery.

### 11. 🤖 [GPAI Model Governance Checklist](templates/gpai-model-governance-checklist.md)
A practical compliance checklist for organizations that develop, fine-tune, or deploy General Purpose AI (GPAI) models under EU AI Act Articles 53–55. Covers the 10^25 FLOPs systemic risk threshold, Article 53 baseline obligations (technical documentation, Annex XI/XII, copyright policy, training data summary), Article 55 systemic risk obligations (adversarial red-teaming, AI Office incident reporting), deployer due diligence requirements, and the GPAI Code of Practice (published July 2025) as a safe-harbor compliance path.

### 12. ⚖️ [Algorithmic Bias Audit Methodology Guide](guides/algorithmic-bias-audit-methodology.md)
A rigorous, step-by-step methodology for conducting an algorithmic fairness audit, grounded in statistical theory and current regulatory requirements. Covers the four core statistical fairness criteria (Demographic Parity, Equal Opportunity, Equalized Odds, Predictive Parity) with exact mathematical definitions; the Chouldechova (2017) and Kleinberg et al. (2016) impossibility theorems and their practical audit implications; a 4-phase audit methodology (pre-audit scoping, data bias audit, model bias audit, intersectional audit); bias mitigation strategies (pre-processing, in-processing, post-processing) with their accuracy-fairness trade-offs; and EU AI Act Article 10 compliance documentation requirements.

## Visual Reference

### Enterprise AI Deployment Tiers
![Enterprise AI Deployment Tiers](assets/deployment-tiers.png)

### EU AI Act Enforcement Timeline
![EU AI Act Enforcement Timeline](assets/eu-ai-act-timeline.png)

---

## How to Use This Framework

For a full walkthrough of every step, see the **[Step-by-Step User Guide](guides/how-to-use-this-framework.md)**. It covers the correct sequence, the responsible owner for each action, and the regulatory rationale behind every tool in this repository.

In brief: start by running the [Shadow AI Risk Calculator](templates/shadow-ai-risk-calculator.md) to quantify your current exposure, then establish the rules with the [Acceptable AI Use Policy](templates/acceptable-use-policy.md), audit your existing vendors with the [Vendor Audit Checklist](templates/vendor-audit-checklist.md), and use the [Deployment Decision Matrix](templates/deployment-decision-matrix.md) to govern every new AI initiative. The sector-specific addenda, DPIA templates, and audit methodology guides apply when you are deploying high-risk AI systems.

## About diShine

At [diShine](https://dishine.it), we build growth architectures and scale revenue for B2B companies. We don't just write policies; we engineer the operational engines that make AI safe and profitable. 

If you need help auditing your current workflows, deploying a private VPC AI environment, or building a custom AI solution that guarantees data sovereignty, [reach out to our team](https://dishine.it/contacts/).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. You are free to use, modify, and distribute these templates within your organization.

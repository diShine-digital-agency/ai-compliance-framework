# AI Compliance Framework for Enterprises

A pragmatic, business-first framework for adopting AI safely in corporate environments without stifling innovation. 

Built by [diShine Digital Agency](https://dishine.it), this repository provides the exact templates, decision matrices, and audit checklists we use to help mid-market and enterprise clients navigate the intersection of the **EU AI Act**, **GDPR**, and corporate **Intellectual Property (IP)** protection.

*Updated: April 2026 — Version 1.2.0*

---

## The Problem: Shadow AI and Regulatory Paralysis

Enterprise AI adoption is currently trapped between two extremes:
1. **Shadow AI:** Employees using consumer-grade tools (like ChatGPT Plus or Claude Pro) without IT oversight, leading to documented IP leaks (e.g., the 2023 Samsung source code incident) and GDPR violations. Gartner estimates that by 2026, 80% of employees will use generative AI for work without company approval.
2. **Regulatory Paralysis:** Legal and compliance teams blocking all AI initiatives due to fear of the EU AI Act (with fines up to €35M or 7% of global turnover) and GDPR enforcement.

**This framework bridges the gap.** It provides the operational guardrails necessary to deploy AI rapidly while maintaining strict data sovereignty and regulatory compliance.

## What's Inside

This repository contains ready-to-use Markdown templates and strategic guidelines:

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

## Visual Reference

### Enterprise AI Deployment Tiers
![Enterprise AI Deployment Tiers](assets/deployment-tiers.png)

### EU AI Act Enforcement Timeline
![EU AI Act Enforcement Timeline](assets/eu-ai-act-timeline.png)

---

## How to Use This Framework

1. **Fork or Clone** this repository.
2. **Adapt the Policy:** Start with the `acceptable-use-policy.md`. Replace the bracketed `[Company Name]` placeholders and adjust the data classification tiers to match your existing infosec policies.
3. **Audit Your Stack:** Use the `vendor-audit-checklist.md` to evaluate any AI tools currently in use (officially or via Shadow IT).
4. **Architect for the Future:** Before approving new AI initiatives, run the use case through the `deployment-decision-matrix.md` to ensure the underlying infrastructure matches the data risk profile.

## About diShine

At [diShine](https://dishine.it), we build growth architectures and scale revenue for B2B companies. We don't just write policies; we engineer the operational engines that make AI safe and profitable. 

If you need help auditing your current workflows, deploying a private VPC AI environment, or building a custom AI solution that guarantees data sovereignty, [reach out to our team](https://dishine.it/contacts/).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details. You are free to use, modify, and distribute these templates within your organization.

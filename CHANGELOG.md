# Changelog

All notable changes to this framework will be documented in this file.

## [2.0.0] - 2026-04-06

### Added

*   `tools/compliance-toolkit.html` — A standalone, client-side web application providing three interactive compliance tools:
    *   **Shadow AI Risk Calculator:** Automated scoring across four dimensions (Organizational Awareness, Technical Controls, Data Governance, Incident History) with section-level breakdowns, risk band determination (Managed / Moderate / Elevated / Critical), and tailored remediation recommendations. Faithfully implements the 100-point scoring system from the framework's Shadow AI Risk Calculator template.
    *   **Vendor Compliance Scorecard:** Interactive 25-item checklist covering GDPR data processing, EU AI Act compliance, and Security & IP requirements. Tracks completion progress, generates pass/fail reports with compliance grades (Strong / Acceptable with Conditions / Significant Gaps / Not Recommended), and identifies specific unmet items.
    *   **Deployment Tier Advisor:** A guided 3-question decision tree that recommends the appropriate deployment architecture (Tier 2 — Enterprise API, Tier 3 — Private Cloud/VPC, or Tier 4 — Self-Hosted) based on data sensitivity, infrastructure capability, and regulatory requirements. Displays detailed tier specifications including cost, GDPR, and EU AI Act considerations.
*   `CONTRIBUTING.md` — Contribution guidelines covering issue reporting, pull request process, content standards, and accepted contribution types.
*   `SECURITY.md` — Security policy with vulnerability reporting process and supported version table.

### Changed

*   `README.md` — Updated to version 2.0.0. Removed marketing language from the introductory paragraph and About section. Replaced "Regulatory Paralysis" framing with "Regulatory Uncertainty" for factual accuracy. Added Interactive Compliance Toolkit as Section 13. Added Contributing and Security sections. Updated How to Use section to reference the interactive toolkit.

### Audit Findings (v2.0.0)

This release was preceded by a full audit of the framework. Key findings:

*   **Regulatory accuracy (9/10):** EU AI Act articles, GDPR references, and sector regulations are correctly cited across all templates.
*   **Template quality:** All 16 templates and guides are relevant, well-structured, and aligned with the April 2026 regulatory landscape.
*   **Scoring inconsistency fixed:** The Shadow AI Risk Calculator's Section D (Incident History) had an ambiguous scoring table where column headers (0/10/20) implied a 40-point max for a 20-point section. The interactive toolkit normalizes this to D1 (0/5/10) + D2 (0/5/10) = 20 points, consistent with the stated section maximum.
*   **Language cleanup:** Removed marketing-oriented phrasing ("business-first," "we engineer operational engines," "bridges the gap") from README in favour of clear, factual descriptions.

## [1.4.1] - 2026-04-06

### Added
- Initial release of the AI Compliance Framework.
- `templates/acceptable-use-policy.md`: Customizable corporate AI use policy.
- `templates/vendor-audit-checklist.md`: 25-point GDPR & EU AI Act vendor evaluation checklist.
- `templates/deployment-decision-matrix.md`: Four-tier enterprise AI deployment decision matrix.
- `templates/prompt-ip-guidelines.md`: Prompt engineering guidelines for IP protection.
- `templates/shadow-ai-risk-calculator.md`: Self-assessment tool for quantifying Shadow AI exposure.
- `assets/deployment-tiers.png`: Visual diagram of the four deployment tiers.
- `assets/eu-ai-act-timeline.png`: Visual timeline of EU AI Act enforcement milestones.

### Regulatory Context (April 2026)
- EU AI Act (Regulation 2024/1689): Prohibited practices (Art. 5) and GPAI obligations (Art. 53) are in force. The majority of remaining rules apply from 2 August 2026.
- The European Commission's Digital Omnibus proposal (November 2025) may delay some high-risk AI system obligations; this framework will be updated once the final text is adopted.
- GDPR remains fully in force; the Italian DPA (Garante) ChatGPT investigation (2023) established precedent for active DPA enforcement against AI tools.

## [1.1.0] - 2026-04-06

### Added
- `templates/dpia-ai-template.md`: Specialized Data Protection Impact Assessment template for AI systems.
- `templates/iso42001-alignment-guide.md`: 12-month implementation roadmap for ISO/IEC 42001:2023 certification.
- `templates/sector-addendum-finance.md`: Regulatory mapping for Financial Services (DORA, MiFID II, Credit Scoring).
- `templates/sector-addendum-tech.md`: Regulatory mapping for Technology companies (Provider vs. Deployer, NIS2, CRA).
- `templates/sector-addendum-beauty.md`: Regulatory mapping for Beauty & Cosmetics (MDR, Biometric Categorization, EU Cosmetics Regulation).

## [1.2.0] - 2026-04-06

### Added

*   `templates/sector-addendum-healthcare.md` — Healthcare & Life Sciences sector addendum covering the MDR/IVDR interaction with the EU AI Act (Annex III.5), GDPR Article 9 special category health data obligations, CDSS-specific requirements (human oversight, explainability, post-market monitoring), and a risk classification matrix with 5 use cases. Includes a clear Deployer vs. Provider obligation breakdown.
*   `templates/sector-addendum-hr.md` — Human Resources & Employment sector addendum covering the EU AI Act Annex III.4 high-risk classification, GDPR Article 22 automated decision-making obligations, EU Employment Equality Directive indirect discrimination risks, the Article 5 prohibition on emotion recognition in the workplace, and Works Council consultation requirements in Germany and France.
*   `templates/dpia-example-library.md` — Pre-filled DPIA example library with three complete, pragmatic examples combining GDPR Article 35 and EU AI Act Article 30 (FRIA) requirements: (1) AI Recruitment Screening Tool with algorithmic bias risk assessment and mandatory human oversight controls; (2) AI Customer Service Chatbot with Sentiment Analysis covering special category data inference and DLP masking measures; (3) AI Employee Performance Monitoring with profiling risk analysis, Works Council consultation requirement, and a mandatory prior Supervisory Authority consultation trigger.

### Changed

*   `README.md` — Updated to version 1.2.0; Healthcare and HR addenda added to the Sector-Specific Addenda section; DPIA Example Library added as a new section (Section 9).

---

## [1.3.0] - 2026-04-06

### Added

*   `templates/ai-incident-response-playbook.md` — A structured, forensic AI incident response framework aligned with EU AI Act Article 73 (Serious Incident Reporting), GDPR Articles 33/34, and the NIST AI RMF 1.0. Includes a P1–P4 severity classification taxonomy, a 6-phase response lifecycle (Preparation, Detection, Containment, Forensic Investigation, Regulatory Notification, Recovery), exact regulatory notification timelines (15-day AI Act window; 2-day window for widespread infringement; 10-day window for death; 72-hour GDPR window), and specific response tactics for prompt injection, model inversion attacks, and algorithmic bias discovery.
*   `templates/gpai-model-governance-checklist.md` — A practical compliance checklist for organizations that develop, fine-tune, or deploy General Purpose AI (GPAI) models under EU AI Act Articles 53–55. Covers the 10^25 FLOPs systemic risk threshold, Article 53 baseline obligations (technical documentation per Annex XI, downstream provider information per Annex XII, copyright compliance policy, mandatory AI Office training data summary template), Article 55 systemic risk obligations (adversarial red-teaming, AI Office incident reporting, cybersecurity measures), deployer due diligence requirements for API users, and the GPAI Code of Practice (published 10 July 2025, endorsed by the AI Board) as a safe-harbor compliance path.

### Changed

*   `README.md` — Updated to version 1.3.0; AI Incident Response Playbook added as Section 10; GPAI Model Governance Checklist added as Section 11.
*   `CHANGELOG.md` — v1.3.0 entry added; Upcoming section updated.

---

## [1.4.0] - 2026-04-06

### Added

*   `guides/algorithmic-bias-audit-methodology.md` — A rigorous, step-by-step algorithmic fairness audit methodology grounded in statistical theory and current regulatory requirements (EU AI Act Article 10, Colorado SB 205, NYC Local Law 144). The guide covers the four core statistical fairness criteria with exact mathematical definitions (Demographic Parity, Equal Opportunity, Equalized Odds, Predictive Parity); the Chouldechova (2017) and Kleinberg et al. (2016) impossibility theorems proving that simultaneous satisfaction of Equalized Odds and Predictive Parity is mathematically impossible when base rates differ; the EU AI Act Article 10(5) legal basis for processing sensitive data strictly for bias correction; a 4-phase audit methodology (pre-audit scoping and legal mapping, data bias audit, model bias audit with disparate impact analysis, intersectional audit); bias mitigation strategies at the pre-processing, in-processing, and post-processing levels with their accuracy-fairness trade-offs; and EU AI Act Annex IV documentation requirements for conformity assessment.

### Changed

*   `README.md` — Updated to version 1.4.0; Algorithmic Bias Audit Methodology Guide added as Section 12.
*   `CHANGELOG.md` — v1.4.0 entry added; Upcoming section updated.

---

## [1.4.1] - 2026-04-06

### Added

*   `guides/how-to-use-this-framework.md` — A comprehensive step-by-step user guide that maps the full AI compliance journey across four phases: (1) Assess & Contain (Shadow AI Risk Calculator, Acceptable Use Policy, Prompt IP Guidelines); (2) Audit & Procure (Vendor Audit Checklist, Sector-Specific Addenda); (3) Architect & Deploy (Deployment Decision Matrix, DPIA, Algorithmic Bias Audit, GPAI Checklist); (4) Monitor & Respond (Incident Response Playbook, ISO 42001 Alignment). Each step names the responsible owner (CISO, DPO, CTO, Legal Counsel, etc.) and explains the regulatory and business rationale behind the action.

### Changed

*   All 16 template and guide files — A contextual "Framework Navigation" footer has been added to each file, identifying which phase and step it belongs to and linking back to the step-by-step user guide.
*   `README.md` — Updated to version 1.4.1; Step-by-Step User Guide added as Section 0 (top of the What's Inside list); "How to Use This Framework" section updated with a link to the full guide.
*   `CHANGELOG.md` — v1.4.1 entry added.

---

## [Upcoming]

*   Sector-specific addenda (Healthcare, HR): ~~pending~~ *(released in v1.2.0)*;
*   DPIA library with pre-filled examples: ~~pending~~ *(released in v1.2.0)*;
*   AI Incident Response Playbook: ~~pending~~ *(released in v1.3.0)*;
*   GPAI (General Purpose AI) model governance checklist: ~~pending~~ *(released in v1.3.0)*;
*   Algorithmic bias audit methodology guide: ~~pending~~ *(released in v1.4.0)*;
*   Step-by-step user guide: ~~pending~~ *(released in v1.4.1)*;
*   Interactive compliance toolkit: ~~pending~~ *(released in v2.0.0)*;
*   AI procurement contract clause library (vendor negotiation templates).

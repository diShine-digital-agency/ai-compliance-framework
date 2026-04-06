# Changelog

All notable changes to this framework will be documented in this file.

## [1.0.0] - 2026-04-06

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

## [Upcoming]

*   Sector-specific addenda (Healthcare, HR): ~~pending~~ *(released in v1.2.0)*;
*   DPIA library with pre-filled examples: ~~pending~~ *(released in v1.2.0)*;
*   AI Incident Response Playbook;
*   GPAI (General Purpose AI) model governance checklist.

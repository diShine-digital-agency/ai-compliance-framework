# Changelog

All notable changes to this framework will be documented in this file.

## [2.1.0] - 2026-04-08

### Added

*   `templates/fria-template.md` — Standalone Fundamental Rights Impact Assessment (FRIA) template implementing EU AI Act Article 27. Covers all relevant EU Charter rights: human dignity (Art. 1), non-discrimination (Art. 21), right to effective remedy (Art. 47), freedom of expression (Art. 11), privacy (Arts. 7–8), right to good administration (Art. 41), workers' rights (Arts. 27–31), rights of children (Art. 24), and rights of persons with disabilities (Art. 26). Includes affected persons analysis, human oversight documentation, MSA notification requirements, and sign-off workflow. Distinct from and complementary to the GDPR DPIA template.
*   `templates/ai-literacy-programme.md` — Practical template for implementing the EU AI Act Article 4 AI literacy obligation (in force since 2 February 2025). Includes a role-based needs assessment matrix (6 role categories from Executive to All Employees), a four-module core curriculum (AI Fundamentals, Regulatory Landscape, Responsible AI for Technical Teams, Human Oversight in Practice), delivery and assessment standards with record-keeping requirements, and guidance on evidencing compliance to national Market Surveillance Authorities.
*   `templates/eu-ai-database-registration-guide.md` — Step-by-step guide for registering high-risk AI systems in the EU AI Database per Article 49. Covers provider, deployer, and Authorised Representative registration obligations, required information per Annex VIII (provider information, AI system details, conformity assessment references), the registration procedure, and penalties for non-registration (up to €15M / 3% of global turnover).
*   `templates/conformity-assessment-guide.md` — Practical guide for high-risk AI system providers navigating the conformity assessment process under Articles 43 and 48, Annexes VI and VII. Explains the two pathways: Internal Control (Annex VI) for most Annex III systems vs. Third-Party Assessment via Notified Body (Annex VII) for regulated products and biometric identification systems. Includes decision flowchart, Quality Management System requirements per Article 17 (10-item checklist), Technical Documentation requirements per Annex IV, CE marking and EU Declaration of Conformity procedures, and Notified Body information.
*   `guides/ai-liability-product-safety.md` — Comprehensive guide to the EU's three-pillar AI liability framework: the EU AI Act (regulatory rules), the AI Liability Directive (COM/2022/496, fault-based liability with rebuttable presumption of causality), and the revised Product Liability Directive (Directive 2024/2853, strict liability extending to software and AI). Covers the transposition deadline (9 December 2026), the new "learning systems" liability provision, burden of proof lightening, disclosure of evidence obligations, and practical implications for both providers (compliance-as-liability-shield, post-deployment monitoring, insurance) and deployers (vendor contracts, human oversight documentation, FRIA as evidence).

### Changed — Content Corrections & European Focus

*   `assets/eu-ai-act-timeline.mmd` — **Major update:** Rebuilt timeline to reflect Digital Omnibus dates. Key changes: high-risk Annex III obligations moved from August 2026 to **2 December 2027**; high-risk regulated products moved to **2 August 2028**; added **2 November 2026** transparency/watermarking deadline; marked already-in-force obligations with ✅; added GPAI Code of Practice (July 2025) milestone.
*   `templates/prompt-ip-guidelines.md` — Removed reference to the US Uniform Trade Secrets Act (UTSA); the primary legal basis is now exclusively the EU Trade Secrets Directive (2016/943), Article 2(1), with correct "reasonable steps" language.
*   `templates/gpai-model-governance-checklist.md` — Corrected "safe-harbor compliance path" to "presumption of compliance" — the legally precise term. Added caveat that the presumption is rebuttable. Updated regulatory context to reference Digital Omnibus timeline revisions.
*   `templates/iso42001-alignment-guide.md` — Corrected the claim that ISO 42001 creates a "presumption of conformity" under EU AI Act Article 40. The correct position: Article 40 refers to harmonised European standards (EN) adopted via CEN/CENELEC, not international standards. ISO 42001 demonstrates "state-of-the-art" governance but does not trigger the Art. 40 presumption.
*   `templates/ai-incident-response-playbook.md` — Replaced NIST AI RMF as the primary alignment framework with EU-native references (ENISA AI Threat Landscape, EU AI Act Articles 9, 12, 61, 72, 73). NIST retained as a complementary international standard. Fixed Article 73 notification timelines to show the multi-step process: initial report without undue delay, full report within 15 days, 2-day accelerated window for widespread fundamental rights infringement, 10-day window for death or imminent death. Added GDPR Article 34 data subject notification obligation.
*   `templates/vendor-audit-checklist.md` — Updated high-risk compliance deadline from "August 2026" to reflect Digital Omnibus timeline. Added risk note on EU-US Data Privacy Framework (DPF) legal fragility following the September 2025 Latombe General Court ruling and anticipated Schrems III challenge; recommends SCCs as parallel safeguard. Removed outdated "Effective Aug 2026" section header.
*   `guides/algorithmic-bias-audit-methodology.md` — Refocused to EU jurisdiction. Removed references to NYC Local Law 144, Colorado SB 205, and EEOC 4/5ths rule. Primary non-discrimination framework is now EU Charter Art. 21, CJEU case law (*Bilka-Kaufhaus v Weber von Hartz*, C-170/84), and EU Employment Equality Directives. Updated references section accordingly.
*   `templates/shadow-ai-risk-calculator.md` — Updated managed-band remediation reference from "2 August 2026" to "2 December 2027" deadline. Added EU-specific enforcement context (Italian Garante fines) alongside global IBM data.
*   `templates/dpia-example-library.md` — Decoupled FRIA from DPIA. Added clear reference to the standalone FRIA template for Article 27 assessments. Updated Example 1 sign-off to reference the separate FRIA.
*   `guides/how-to-use-this-framework.md` — Updated to v2.1.0. Added four new steps: Step 1.4 (AI Literacy), Step 2.3 (AI Liability Exposure), Step 3.5 (FRIA), Step 3.6 (EU AI Database Registration), Step 3.7 (Conformity Assessment & CE Marking). Updated Step 4.2 to correct ISO 42001 conformity presumption language. Added links to Technology and Beauty sector addenda in Step 2.2.
*   `README.md` — Updated to version 2.1.0. Corrected EU AI Act penalty structure to show all three tiers (€35M/7%, €15M/3%, €7.5M/1%). Updated Incident Response Playbook description to reference ENISA instead of NIST. Updated GPAI checklist description from "safe-harbor" to "presumption-of-compliance." Updated DPIA Example Library description to separate FRIA. Added new documents as Sections 14–18. Updated How to Use section with links to new templates.

### Regulatory Context (April 2026)

*   The Digital Omnibus proposal (November 2025) is in the final trilogue stage (Council adopted position 13 March 2026; Parliament adopted position 26 March 2026; second trilogue scheduled for 28 April 2026). Key timeline changes are reflected throughout this framework with a caveat that final adoption is pending.
*   The GPAI Code of Practice was published in final form on 10 July 2025 and is now the primary voluntary compliance instrument for GPAI providers.
*   The EU-US Data Privacy Framework (DPF) was upheld by the EU General Court in September 2025 (Latombe case), but significant legal uncertainty remains. A Schrems III challenge is anticipated.
*   The revised Product Liability Directive (2024/2853) must be transposed by Member States by 9 December 2026.
*   Finland became the first Member State to activate national AI Act supervision (January 2026).

## [2.0.0] - 2026-04-06

### Added

*   `tools/compliance-toolkit.html` — A standalone, client-side web application providing three interactive compliance tools:
    *   **Shadow AI Risk Calculator:** Automated scoring across four dimensions (Organizational Awareness, Technical Controls, Data Governance, Incident History) with section-level breakdowns, risk band determination (Managed / Moderate / Elevated / Critical), and tailored remediation recommendations. Faithfully implements the 100-point scoring system from the framework's Shadow AI Risk Calculator template.
    *   **Vendor Compliance Scorecard:** Interactive 25-item checklist covering GDPR data processing, EU AI Act compliance, and Security & IP requirements. Tracks completion progress, generates pass/fail reports with compliance grades (Strong / Acceptable with Conditions / Significant Gaps / Not Recommended), and identifies specific unmet items.
    *   **Deployment Tier Advisor:** A guided 3-question decision tree that recommends the appropriate deployment architecture (Tier 2 — Enterprise API, Tier 3 — Private Cloud/VPC, or Tier 4 — Self-Hosted) based on data sensitivity, infrastructure capability, and regulatory requirements. Displays detailed tier specifications including cost, GDPR, and EU AI Act considerations.
*   `CONTRIBUTING.md` — Contribution guidelines covering issue reporting, pull request process, content standards, and accepted contribution types.
*   `SECURITY.md` — Security policy with vulnerability reporting process and supported version table.

### Changed

*   `README.md` — Updated to version 2.0.0. Cleaned language from the introductory paragraph and About section. Replaced "Regulatory Paralysis" framing with "Regulatory Uncertainty" for factual accuracy. Added Interactive Compliance Toolkit as Section 13. Added Contributing and Security sections. Updated How to Use section to reference the interactive toolkit.

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
- EU AI Act (Regulation 2024/1689): Prohibited practices (Art. 5), AI literacy (Art. 4), and GPAI obligations (Art. 53) are in force. Transparency obligations apply from 2 November 2026. High-risk Annex III obligations apply from 2 December 2027 (as revised by the Digital Omnibus).
- The European Commission's Digital Omnibus proposal (November 2025) has revised high-risk AI system deadlines; the Council and Parliament have adopted positions (March 2026) and the final trilogue text is expected by late April 2026.
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
*   `templates/gpai-model-governance-checklist.md` — A practical compliance checklist for organizations that develop, fine-tune, or deploy General Purpose AI (GPAI) models under EU AI Act Articles 53–55. Covers the 10^25 FLOPs systemic risk threshold, Article 53 baseline obligations (technical documentation per Annex XI, downstream provider information per Annex XII, copyright compliance policy, mandatory AI Office training data summary template), Article 55 systemic risk obligations (adversarial red-teaming, AI Office incident reporting, cybersecurity measures), deployer due diligence requirements for API users, and the GPAI Code of Practice (published 10 July 2025, endorsed by the AI Board) as a presumption-of-compliance path.

### Changed

*   `README.md` — Updated to version 1.3.0; AI Incident Response Playbook added as Section 10; GPAI Model Governance Checklist added as Section 11.
*   `CHANGELOG.md` — v1.3.0 entry added; Upcoming section updated.

---

## [1.4.0] - 2026-04-06

### Added

*   `guides/algorithmic-bias-audit-methodology.md` — A rigorous, step-by-step algorithmic fairness audit methodology grounded in statistical theory and current EU regulatory requirements (EU AI Act Article 10, EU Charter Art. 21, EU Employment Equality Directives). The guide covers the four core statistical fairness criteria with exact mathematical definitions (Demographic Parity, Equal Opportunity, Equalized Odds, Predictive Parity); the Chouldechova (2017) and Kleinberg et al. (2016) impossibility theorems proving that simultaneous satisfaction of Equalized Odds and Predictive Parity is mathematically impossible when base rates differ; the EU AI Act Article 10(5) legal basis for processing sensitive data strictly for bias correction; a 4-phase audit methodology (pre-audit scoping and legal mapping, data bias audit, model bias audit with disparate impact analysis, intersectional audit); bias mitigation strategies at the pre-processing, in-processing, and post-processing levels with their accuracy-fairness trade-offs; and EU AI Act Annex IV documentation requirements for conformity assessment.

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
*   FRIA template, AI Literacy programme, EU AI Database guide, Conformity Assessment guide, AI Liability guide: ~~pending~~ *(released in v2.1.0)*;
*   AI procurement contract clause library (vendor negotiation templates);
*   Sector addenda for Education, Law Enforcement, Public Administration, Energy/Critical Infrastructure.

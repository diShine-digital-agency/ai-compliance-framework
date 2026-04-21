# Changelog

All notable changes to this framework will be documented in this file.

## [2.3.0] - 2026-04-20

### Changed — April 2026 Content Audit, Omnibus-Aware Dating & Regulatory De-risking

This release corrects licensing metadata, propagates the Digital Omnibus enforcement calendar across the wiki knowledge base and removes residual US-centric legal references.

**Licensing & versioning**

*   `README.md` — Fixed broken license badge (previously showed "CC0 1.0"; actual project license is MIT). Bumped header version to 2.3.0. Added a prominent Digital Omnibus status caveat so readers understand why two enforcement timelines coexist in the documentation.
*   `CHANGELOG.md` — Corrected a duplicate `[1.4.1]` entry: the "Initial release" block (2026-04-06) has been renumbered to `[1.0.0]` to reflect what it actually represents (the first public release). The genuine `[1.4.1]` entry (Step-by-Step User Guide, Framework Navigation footers) is retained.
*   `PLD transposition date` — Standardised as **9 December 2026** across `README.md`, `guides/how-to-use-this-framework.md`, `wiki/AI-Liability-in-the-EU.md`, and `wiki/EU-Regulatory-Landscape-for-AI.md` (previously rendered as "December 2026").

**Omnibus-aware enforcement dating — wiki knowledge base**

Every wiki page that cited a single "2 August 2026" deadline for Annex III high-risk obligations now reflects the Digital Omnibus proposed timeline (**2 December 2027**) while preserving the pre-Omnibus legally binding date (**2 August 2026**) and directing readers to the Enforcement Timeline page for canonical status.

*   `wiki/EU-AI-Act-Enforcement-Timeline.md` — Fully rewritten. New at-a-glance timeline graphic, 2024/2025/2026/2027/2028/2030 detailed date tables, Digital Omnibus legislative-status section with trilogue dates (Council 13 March 2026, EP 26 March 2026, trilogue 28 April 2026, OJ publication targeted July 2026), and a status caveat clarifying that pre-Omnibus dates remain legally binding until publication.
*   `wiki/High-Risk-AI-Systems.md` — Replaced "2 August 2026" with Omnibus-aware wording referencing 2 December 2027 with the pre-Omnibus caveat and a cross-link to the Enforcement Timeline.
*   `wiki/EU-AI-Act-Risk-Classification.md` — Updated the high-risk entry-into-force paragraph; added the 2 August 2028 regulated-products date for legacy systems.
*   `wiki/EU-AI-Database-Registration.md` — Updated the Article 49 effective-date paragraph and the timeline table (new registrations: 2 Dec 2027 / regulated products: 2 Aug 2028).
*   `wiki/Harmonised-Standards.md` — Rewrote the "Compliance Gap" section to show both the 2 August 2026 (pre-Omnibus) and 2 December 2027 (Omnibus) milestones and clarified that the 2027 target for standards publication now aligns with the Omnibus binding date.
*   `wiki/EU-AI-Act-Penalties-and-Fines.md` — Updated the Penalty Timeline entry for full-regime activation to show both dates.
*   `wiki/Transparency-Obligations.md` — Corrected Article 50 effective date to **2 November 2026** (Omnibus) with the pre-Omnibus caveat.
*   `wiki/General-Purpose-AI-GPAI.md` — Fixed incorrect statement that GPAI enforcement "becomes available from 2 August 2026"; enforcement powers and the GPAI penalty regime have been active since **2 August 2025**.
*   `wiki/FAQ.md` — Updated the entry-into-force, regulatory-sandbox, and harmonised-standards Q&A entries with Omnibus-aware dates.
*   `wiki/AI-Governance-and-Board-Oversight.md` — Updated the board-reporting and AI-governance-committee cadence references to reflect the dual-date regime.
*   `wiki/Regulatory-Sandboxes.md` — Clarified that the 2 August 2026 Article 57 sandbox deadline is **retained under the Digital Omnibus proposal** (unlike the high-risk and Article 50 dates).
*   `wiki/EU-Regulatory-Landscape-for-AI.md` — Applied the same sandbox clarification; standardised the PLD date.
*   `wiki/AI-Liability-in-the-EU.md` — Standardised the PLD transposition date to 9 December 2026.

**Residual US references removed (EU-native focus)**

The v2.1.0 release removed the bulk of US regulatory references from the bias-audit and incident-response materials. This release cleans up the residuals that remained in the wiki and in one template header.

*   `templates/ai-incident-response-playbook.md` — Removed the NIST AI RMF 1.0 sentence from the alignment statement. The playbook is now framed purely against EU AI Act Art. 73, GDPR Arts. 33/34, and the ENISA AI Threat Landscape.
*   `wiki/AI-Incident-Response.md` — Removed NIST AI RMF from the framework alignment list.
*   `wiki/Key-Regulatory-References.md` — Replaced the NIST AI RMF row in the "Industry Frameworks" table with the GPAI Code of Practice, ENISA AI Threat Landscape, OECD AI Principles, and ISO/IEC 42001 to give an EU-first reference list.
*   `wiki/ISO-42001-and-AI-Governance-Standards.md` — Removed the NIST AI RMF row from the related-standards table.
*   `guides/algorithmic-bias-audit-methodology.md` — Removed references to the "80% rule" / four-fifths rule (a US EEOC construct) from the introduction; replaced with an EU-native framing anchored on the CJEU *Bilka-Kaufhaus* indirect-discrimination standard (Case C-170/84) and the EU Employment Equality Directives. Rewrote the post-processing mitigation caveat in EU non-discrimination terms (positive-action justification) rather than the US "disparate impact/disparate treatment" dichotomy.
*   `wiki/Algorithmic-Bias-and-Fairness.md` — Replaced "80% rule / four-fifths rule for disparate impact" references in the pre-audit and model-audit phases with EU-law-anchored wording (CJEU case law, statistically significant adverse impact).

**Documentation handoff files added**

*   `CHANGES-FOR-LOVABLE.md` — Page-level change instructions for the companion SPA at [aicompliance.dishine.it](https://aicompliance.dishine.it). Maps each content change to the corresponding route (`/`, `/framework`, `/playbook`, `/toolkit`, `/wiki`, `/about`, `/wiki/<slug>`).
*   `CHANGES-FOR-COPILOT.md` — File-level change instructions for GitHub Copilot to replay the edits on the GitHub Wiki repository (`ai-compliance-framework.wiki.git`). Includes exact file paths, before/after strings, and validation commands.

**New canonical home — [compliance.dishine.it](https://compliance.dishine.it)**

The framework now has a dedicated website. Going forward, primary content updates will be published on the site first; the GitHub repository remains actively maintained as the open collaboration space for issues, pull requests, forks, and discussion. Prominent "new home" notices were added across the documentation so this model is unambiguous to any reader landing on the repo or wiki.

*   `README.md` — Added a prominent "new home" notice directly below the Digital Omnibus caveat. Removed the two ad-hoc one-line references to `compliance.dishine.it` (previously above "Visual reference" and next to the "More details" heading) now that the consolidated notice replaces them.
*   `CONTRIBUTING.md` — Added a "new home & contribution model" notice at the top clarifying that the site is the canonical version for readers, and that issues, pull requests, forks, and discussion happen in the repo.
*   `wiki/Home.md` — Added a "new home" notice under the wiki intro paragraph.
*   `wiki/About-This-Framework.md` — Added a "new home" notice at the top and rewrote the "Relationship Between Repository and Wiki" section into "Relationship Between the Website, the Repository, and the Wiki" to describe the three-surface model.
*   `guides/how-to-use-this-framework.md` — Added a "new home" notice directly below the version line and bumped the stated version from `2.2.1` to `2.3.0` to align with the release metadata.

### Regulatory Context (April 2026)

*   The Digital Omnibus on AI Regulation remains in trilogue as of this release. Trilogue political agreement is expected 28 April 2026; publication in the Official Journal is targeted for July 2026. Until then, the original Regulation 2024/1689 dates (notably 2 August 2026 for Annex III and Article 50) remain legally binding.
*   The revised Product Liability Directive (2024/2853) transposition deadline is **9 December 2026**.
*   The GPAI Code of Practice final version (**10 July 2025**) remains the primary voluntary compliance instrument for GPAI providers and provides a rebuttable presumption of compliance.

## [2.2.1] - 2026-04-08

### Added — In-Depth Wiki Knowledge Base

*   **`wiki/` directory (42 pages)** — A comprehensive, in-depth knowledge base covering the full scope of EU AI regulation and practical compliance guidance. The wiki complements the repository's templates, guides, and tools with deep regulatory explanations, process walkthroughs, and cross-referenced reference material. It is automatically synced to the [GitHub Wiki](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki) via the `sync-wiki.yml` GitHub Actions workflow.

    **EU AI Act — Core Concepts (12 pages):**
    *   `EU-AI-Act-Overview.md` — Structure, scope, and objectives of Regulation (EU) 2024/1689.
    *   `EU-AI-Act-Risk-Classification.md` — The four-tier risk model (Unacceptable, High, Limited, Minimal).
    *   `EU-AI-Act-Enforcement-Timeline.md` — All key compliance dates from August 2024 through August 2027.
    *   `EU-AI-Act-Penalties-and-Fines.md` — The three-tier penalty structure and fine calculation.
    *   `EU-AI-Act-Roles.md` — Provider, Deployer, Importer, Distributor obligations.
    *   `Prohibited-AI-Practices.md` — Article 5 prohibitions effective since February 2025.
    *   `High-Risk-AI-Systems.md` — Annex III use cases, Articles 9–15 requirements, conformity assessment.
    *   `General-Purpose-AI-GPAI.md` — Articles 51–55, systemic risk, GPAI Code of Practice.
    *   `Transparency-Obligations.md` — Article 50 disclosure, content labelling, deepfake rules.
    *   `Conformity-Assessment.md` — Internal control vs. Notified Body pathways.
    *   `EU-AI-Database-Registration.md` — Article 49 registration obligations.
    *   `Post-Market-Monitoring.md` — Article 72 continuous monitoring obligations.

    **Related EU Regulations (7 pages):**
    *   `GDPR-and-AI.md` — GDPR intersection with AI systems.
    *   `EU-Regulatory-Landscape-for-AI.md` — AI Act interaction with NIS2, DORA, CRA, DSA, and PLD.
    *   `AI-Liability-in-the-EU.md` — Three-pillar liability framework (AI Act, AILD, revised PLD).
    *   `National-Implementation.md` — Member State progress on competent authority designation.
    *   `Regulatory-Sandboxes.md` — Article 57 supervised testing environments.
    *   `Harmonised-Standards.md` — CEN/CENELEC standardisation and presumption of conformity.
    *   `Open-Source-AI-and-the-EU-AI-Act.md` — Scope and limits of the open-source exemption.

    **Compliance Processes (8 pages):**
    *   `DPIA-for-AI.md` — Data Protection Impact Assessment adapted for AI (GDPR Article 35).
    *   `Fundamental-Rights-Impact-Assessment.md` — EU AI Act Article 27 FRIA.
    *   `Shadow-AI.md` — Risks of unsanctioned AI use and mitigation strategies.
    *   `AI-Vendor-Due-Diligence.md` — Evaluating third-party AI vendors for GDPR/AI Act compliance.
    *   `Algorithmic-Bias-and-Fairness.md` — Fairness metrics, impossibility theorems, audit methodology.
    *   `AI-Incident-Response.md` — Detecting, containing, and reporting AI-related incidents.
    *   `AI-Literacy-Obligation.md` — Article 4 requirements effective since February 2025.
    *   `IP-Protection-and-AI.md` — Protecting intellectual property and trade secrets when using AI.

    **Standards & Governance (2 pages):**
    *   `ISO-42001-and-AI-Governance-Standards.md` — ISO/IEC 42001:2023 and its EU AI Act relationship.
    *   `AI-Governance-and-Board-Oversight.md` — Board-level accountability, governance committees, AI risk registers.

    **Sector-Specific Guides (7 pages):**
    *   `Sector-Guide-Financial-Services.md` — DORA, MiFID II, credit scoring, insurance pricing.
    *   `Sector-Guide-Healthcare.md` — MDR/IVDR, clinical decision support, health data governance.
    *   `Sector-Guide-Human-Resources.md` — Recruitment AI, performance monitoring, worker rights.
    *   `Sector-Guide-Technology.md` — Provider vs. Deployer, NIS2, CRA, SaaS obligations.
    *   `Sector-Guide-Beauty-and-Cosmetics.md` — Virtual try-on, skin analysis, biometric rules.
    *   `Sector-Guide-Education.md` — Admissions AI, automated grading, exam proctoring, student data.
    *   `Sector-Guide-Public-Administration.md` — Government AI, social benefits, law enforcement, public-sector FRIA.

    **Reference (3 pages):**
    *   `Glossary.md` — 14+ key terms with definitions sourced from the EU AI Act, GDPR, and related legislation.
    *   `Key-Regulatory-References.md` — Official regulatory texts, guidance documents, and authoritative sources.
    *   `FAQ.md` — 7+ categories of frequently asked questions covering the framework, EU AI Act, risk classification, GDPR, practical compliance, sector-specific rules, and transparency.

    **Framework & Repository (3 pages):**
    *   `Home.md` — Wiki landing page with navigation and reading guidance.
    *   `About-This-Framework.md` — What the framework is, who it serves, and how it was built.
    *   `Repository-Guide.md` — Complete file-by-file reference of every template, guide, and tool.

*   `.github/workflows/sync-wiki.yml` — GitHub Actions workflow that automatically synchronises the `wiki/` directory to the GitHub Wiki on every push to `main` that modifies wiki files. Supports manual dispatch.

### Changed

*   `README.md` — Updated to version 2.2.1. Added comprehensive "Wiki — In-Depth Knowledge Base" section with categorised links to all 42 wiki pages. Added note on automatic wiki synchronisation from the `wiki/` directory.
*   `guides/how-to-use-this-framework.md` — Updated to version 2.2.1. Added wiki cross-reference directing users to the knowledge base for regulatory background.
*   `CONTRIBUTING.md` — Added wiki contributions as an accepted contribution type with guidance on file naming and cross-linking conventions.
*   `wiki/Repository-Guide.md` — Updated directory structure to include the `wiki/` directory listing and `sync-wiki.yml` workflow.

## [2.2.0] - 2026-04-08

### Changed — April 2026 Enforcement Updates & Content Audit

*   `tools/compliance-toolkit.html` — Fixed outdated date in Shadow AI Risk Calculator "Managed" remediation text: changed "2 August 2026 EU AI Act deadline" to "2 December 2027" to match the Digital Omnibus timeline correction applied to the Markdown templates in v2.1.0.
*   `templates/gpai-model-governance-checklist.md` — Added reference to the GPAI Code of Practice v2.1 (released 3 April 2026) with strengthened training data summary requirements and standardised format.
*   `templates/ai-incident-response-playbook.md` — Added note on the Irish DPC's first formal Article 11 documentation request (April 2026) against a SaaS candidate-screening tool, signalling active enforcement.
*   `templates/conformity-assessment-guide.md` — Added reference to the EU AI Office standardised documentation templates (released April 2026), now the practical benchmark for MSA compliance audits.
*   `templates/acceptable-use-policy.md` — Added reference to the European Commission's updated Article 5 prohibited practices guidance (published 2 April 2026), expanding the scope of "subliminal techniques" to include recommender systems using hidden user signals for nudging.
*   `templates/iso42001-alignment-guide.md` — Added reference to Europrivacy certification as an emerging pathway for demonstrating integrated AI Act and GDPR compliance.
*   `SECURITY.md` — Updated supported versions table from "2.0.x" to "2.x.x" to correctly reflect the v2.1.0+ release.

### Regulatory Context (April 2026)

*   The Irish Data Protection Commission issued the first formal Article 11 documentation request under the EU AI Act, targeting a SaaS provider of a candidate-screening AI tool. This is the first known active enforcement action under the AI Act's technical documentation obligations.
*   The European Commission published updated guidance on Article 5 prohibited practices (2 April 2026), clarifying the prohibition on "subliminal techniques" — specifically, recommender systems using hidden user signals for nudging must now perform and document a "user-interest test."
*   The GPAI Code of Practice v2.1 was released on 3 April 2026, strengthening the training data summary requirements with a new standardised format template from the AI Office.
*   The EU AI Office released standardised documentation templates that national Market Surveillance Authorities are now using as the benchmark for compliance audits. These templates align with Annex IV requirements and should be adopted by all providers of high-risk AI systems.
*   Europrivacy certification is emerging as an efficient pathway for demonstrating integrated compliance with both the AI Act and GDPR.
*   The `eu-ai-act-timeline.png` diagram needs regeneration from the updated `eu-ai-act-timeline.mmd` source file to reflect Digital Omnibus dates (requires Mermaid CLI or a Mermaid renderer).

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
*   Sector addenda for Education, Law Enforcement, Public Administration, Energy/Critical Infrastructure;
*   Regenerate `eu-ai-act-timeline.png` from the updated Mermaid source to reflect Digital Omnibus dates;
*   Integration of EU AI Office standardised documentation templates as downloadable annexes.

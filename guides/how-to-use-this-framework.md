# How to Use the AI Compliance Framework: A Step-by-Step Guide

**Version:** 2.2.1

This framework is not a collection of isolated documents; it is a sequential, operational engine designed to move an enterprise from "Shadow AI chaos" to "auditable, compliant AI deployment" under the EU AI Act and GDPR. 

This guide explains the exact sequence in which to deploy these tools, why each step matters, and who should own it.

> **📚 Need regulatory background?** The [AI Compliance Framework Wiki](https://github.com/diShine-digital-agency/ai-compliance-framework/wiki) provides in-depth explanations of the EU AI Act, GDPR, related regulations, and compliance processes referenced throughout this guide.

---

## Phase 1: Assess & Contain (Days 1–14)

Before you can build compliant AI, you must stop the bleeding. Employees are already using consumer-grade AI tools, and your intellectual property is likely already exposed.

### Step 1.1: Quantify the Current Risk
*   **Tool:** [`templates/shadow-ai-risk-calculator.md`](../templates/shadow-ai-risk-calculator.md), or use the Shadow AI Risk Calculator
 in the client-side web application by opening the file `compliance-toolkit.html` in the folder [`TOOLS`](../tools/).
*   **Owner:** Chief Information Security Officer (CISO) or IT Director.
*   **Why it matters:** You cannot secure budget or executive buy-in for an AI governance program without quantifying the current exposure. This 100-point calculator translates vague fears about "Shadow AI" into a concrete risk score based on IBM and Gartner benchmarks.
*   **Action:** Run the assessment. If you score above 50 (Elevated Risk), proceed immediately to Step 1.2.

### Step 1.2: Establish the Baseline Rules
*   **Tool:** [`templates/acceptable-use-policy.md`](../templates/acceptable-use-policy.md)
*   **Owner:** Legal Counsel & HR.
*   **Why it matters:** If an employee uploads confidential source code to a public LLM, you cannot discipline them or claim a trade secret violation unless a formal policy explicitly forbade it. 
*   **Action:** Customize the bracketed `[Company Name]` fields, align the data classification tiers (Public, Internal, Confidential, Restricted) with your existing infosec policy, and distribute it company-wide via HR.

### Step 1.3: Secure the Prompts
*   **Tool:** [`templates/prompt-ip-guidelines.md`](../templates/prompt-ip-guidelines.md)
*   **Owner:** Engineering Leads & Product Managers.
*   **Why it matters:** Even when using approved enterprise APIs, poorly constructed prompts can leak PII or proprietary logic.
*   **Action:** Integrate these guidelines into your developer onboarding and code review processes.

### Step 1.4: Implement AI Literacy (Article 4)
*   **Tool:** [`templates/ai-literacy-programme.md`](../templates/ai-literacy-programme.md)
*   **Owner:** HR & Legal Counsel.
*   **Why it matters:** Article 4 of the EU AI Act (in force since February 2025) requires **all** providers and deployers to ensure their staff have sufficient AI literacy, proportionate to their role and the AI systems they interact with. This is a horizontal obligation — it applies regardless of risk classification.
*   **Action:** Customise the role-based curriculum, deliver the foundational modules company-wide, and maintain a training register as evidence of compliance.

---

## Phase 2: Audit & Procure (Days 15–45)

Once the bleeding is stopped, you must evaluate the third-party AI tools your company is already paying for, and establish a gate for new ones.

### Step 2.1: Audit Existing Vendors
*   **Tool:** [`templates/vendor-audit-checklist.md`](../templates/vendor-audit-checklist.md), or use the Vendor Audit Scorecard in the client-side web application by opening the file `compliance-toolkit.html` in the folder [`TOOLS`](../tools/).
*   **Owner:** Procurement & Data Protection Officer (DPO).
*   **Why it matters:** Under GDPR Article 28 and the EU AI Act, you (the Deployer/Controller) are liable for the compliance of your vendors (the Providers/Processors). A standard SOC2 questionnaire does not cover AI-specific risks like training data provenance or automated decision-making.
*   **Action:** Send this 25-point checklist to every vendor currently providing AI capabilities (e.g., your ATS, your CRM, your customer support platform).

### Step 2.2: Map Sector-Specific Obligations
*   **Tool:** `templates/sector-addendum-[industry].md` (e.g., [Finance](../templates/sector-addendum-finance.md), [Healthcare](../templates/sector-addendum-healthcare.md), [HR](../templates/sector-addendum-hr.md), [Technology](../templates/sector-addendum-tech.md), [Beauty](../templates/sector-addendum-beauty.md))
*   **Owner:** Legal Counsel.
*   **Why it matters:** The EU AI Act does not exist in a vacuum. It intersects with existing sectoral laws (MDR for healthcare, DORA for finance). 
*   **Action:** Read the relevant addendum to understand if your specific use cases trigger Annex III high-risk classifications or require prior Supervisory Authority consultation.

### Step 2.3: Understand AI Liability Exposure
*   **Tool:** [`guides/ai-liability-product-safety.md`](ai-liability-product-safety.md)
*   **Owner:** Legal Counsel & Risk Management.
*   **Why it matters:** The EU AI Act sets rules, but the revised **Product Liability Directive** (2024/2853, transposition deadline December 2026) and the proposed **AI Liability Directive** create private rights of action for individuals harmed by AI. Non-compliance with the AI Act triggers a presumption of causality in liability claims.
*   **Action:** Review the three-pillar liability framework. Update vendor contracts with liability allocation and indemnification clauses. Assess whether AI-specific product liability insurance is needed.

---

## Phase 3: Architect & Deploy (Days 45–90)

When the business demands a new, custom AI capability, IT must decide how to build it safely.

### Step 3.1: Choose the Deployment Architecture
*   **Tool:** [`templates/deployment-decision-matrix.md`](../templates/deployment-decision-matrix.md), or use the Deployment Tier Advisor in the client-side web application by opening the file `compliance-toolkit.html` in the folder [`TOOLS`](../tools/).
*   **Owner:** Chief Technology Officer (CTO) or Chief Architect.
*   **Why it matters:** Not every AI project needs a self-hosted Llama 3 model, and not every project is safe for the OpenAI public API. This matrix forces a structured decision based on data sensitivity and latency requirements.
*   **Action:** Require a completed decision matrix as part of the technical design document for any new AI initiative.

### Step 3.2: Conduct the Impact Assessment
*   **Tool:** [`templates/dpia-ai-template.md`](../templates/dpia-ai-template.md) (Reference the [`templates/dpia-example-library.md`](../templates/dpia-example-library.md) for guidance)
*   **Owner:** DPO & Product Owner.
*   **Why it matters:** GDPR Article 35 mandates a DPIA for processing that is "likely to result in a high risk," which almost all consequential AI systems do.
*   **Action:** Complete the DPIA *before* any code is written or data is processed.

### Step 3.3: Audit for Algorithmic Bias
*   **Tool:** [`guides/algorithmic-bias-audit-methodology.md`](algorithmic-bias-audit-methodology.md)
*   **Owner:** Lead Data Scientist & Compliance Officer.
*   **Why it matters:** If your system makes decisions about humans (credit, employment, housing), it will be scrutinised for bias under EU AI Act Article 10 and the EU Employment Equality Directives.
*   **Action:** Follow the 4-phase methodology to select a fairness metric, test the model, and document the accuracy-fairness trade-off for the Annex IV technical documentation.

### Step 3.4: GPAI Governance (If Applicable)
*   **Tool:** [`templates/gpai-model-governance-checklist.md`](../templates/gpai-model-governance-checklist.md)
*   **Owner:** AI Engineering Lead.
*   **Why it matters:** If you are fine-tuning a General Purpose AI model or building one from scratch, you may trigger Article 53-55 obligations.
*   **Action:** Run the checklist to determine if you cross the 10^25 FLOPs systemic risk threshold and to ensure Annex XI/XII documentation is complete.

### Step 3.5: Conduct the Fundamental Rights Impact Assessment (FRIA)
*   **Tool:** [`templates/fria-template.md`](../templates/fria-template.md)
*   **Owner:** Legal Counsel & DPO.
*   **Why it matters:** Article 27 of the EU AI Act requires deployers of high-risk AI systems to conduct a FRIA **before** putting the system into use. This is **separate from the GDPR DPIA** — it assesses impact on fundamental rights under the EU Charter (dignity, non-discrimination, effective remedy, workers' rights, etc.), not just data protection.
*   **Action:** Complete the FRIA template for each high-risk AI system. Submit results to the national Market Surveillance Authority as part of the EU AI Database registration.

### Step 3.6: Register in the EU AI Database
*   **Tool:** [`templates/eu-ai-database-registration-guide.md`](../templates/eu-ai-database-registration-guide.md)
*   **Owner:** Legal Counsel & AI Engineering Lead.
*   **Why it matters:** Article 49 requires providers and deployers of high-risk AI systems to register in the EU AI Database **before** the system is placed on the market or put into service. Failure to register carries fines of up to €15M / 3% of turnover.
*   **Action:** Follow the step-by-step registration procedure. Prepare all required documentation (Technical Documentation, EU Declaration of Conformity, FRIA results for public-sector deployers).

### Step 3.7: Conformity Assessment & CE Marking (Providers Only)
*   **Tool:** [`templates/conformity-assessment-guide.md`](../templates/conformity-assessment-guide.md)
*   **Owner:** Quality Assurance & Legal Counsel.
*   **Why it matters:** Providers of high-risk AI systems must complete a conformity assessment and affix the CE mark before placing the system on the EU market. The pathway depends on whether the AI is a standalone Annex III system (Internal Control) or a safety component of a regulated product (Notified Body).
*   **Action:** Use the decision flowchart to determine the correct pathway. Implement the Quality Management System (Article 17) and prepare Technical Documentation (Annex IV).

---

## Phase 4: Monitor & Respond (Ongoing)

AI systems degrade over time (concept drift) and are subject to novel attack vectors (prompt injection).

### Step 4.1: Prepare for Incidents
*   **Tool:** [`templates/ai-incident-response-playbook.md`](../templates/ai-incident-response-playbook.md)
*   **Owner:** Security Operations Center (SOC) & Incident Response Team.
*   **Why it matters:** When an AI model hallucinates a defamatory statement or leaks PII, the standard IT incident response playbook will fail. You need specific containment tactics that preserve model weights for forensic investigation.
*   **Action:** Integrate this playbook into your existing SIEM/SOAR workflows and conduct a tabletop exercise.

### Step 4.2: Align with Global Standards
*   **Tool:** [`templates/iso42001-alignment-guide.md`](../templates/iso42001-alignment-guide.md)
*   **Owner:** Head of Compliance / Quality Assurance.
*   **Why it matters:** ISO/IEC 42001:2023 is the globally recognised standard for AI Management Systems. While it does not automatically create a presumption of conformity under the EU AI Act (that requires harmonised European standards via CEN/CENELEC), it demonstrates "state-of-the-art" governance.
*   **Action:** Use the 12-month roadmap to formalise your AI governance into a certifiable management system.

---

*This guide is part of the AI Compliance Framework by diShine Digital Agency.*

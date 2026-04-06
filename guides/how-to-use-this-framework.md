# How to Use the AI Compliance Framework: A Step-by-Step Guide

**Version:** 1.4.1

This framework is not a collection of isolated documents; it is a sequential, operational engine designed to move an enterprise from "Shadow AI chaos" to "auditable, compliant AI deployment" under the EU AI Act and GDPR. 

This guide explains the exact sequence in which to deploy these tools, why each step matters, and who should own it.

---

## Phase 1: Assess & Contain (Days 1–14)

Before you can build compliant AI, you must stop the bleeding. Employees are already using consumer-grade AI tools, and your intellectual property is likely already exposed.

### Step 1.1: Quantify the Current Risk
*   **Tool:** [`templates/shadow-ai-risk-calculator.md`](../templates/shadow-ai-risk-calculator.md) or use the standalone, client-side web application by opening the file `compliance-toolkit.html` in the folder [`TOOLS`](../tools/).
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

---

## Phase 2: Audit & Procure (Days 15–45)

Once the bleeding is stopped, you must evaluate the third-party AI tools your company is already paying for, and establish a gate for new ones.

### Step 2.1: Audit Existing Vendors
*   **Tool:** [`templates/vendor-audit-checklist.md`](../templates/vendor-audit-checklist.md)
*   **Owner:** Procurement & Data Protection Officer (DPO).
*   **Why it matters:** Under GDPR Article 28 and the EU AI Act, you (the Deployer/Controller) are liable for the compliance of your vendors (the Providers/Processors). A standard SOC2 questionnaire does not cover AI-specific risks like training data provenance or automated decision-making.
*   **Action:** Send this 25-point checklist to every vendor currently providing AI capabilities (e.g., your ATS, your CRM, your customer support platform).

### Step 2.2: Map Sector-Specific Obligations
*   **Tool:** `templates/sector-addendum-[industry].md` (e.g., [Finance](../templates/sector-addendum-finance.md), [Healthcare](../templates/sector-addendum-healthcare.md), [HR](../templates/sector-addendum-hr.md))
*   **Owner:** Legal Counsel.
*   **Why it matters:** The EU AI Act does not exist in a vacuum. It intersects with existing sectoral laws (MDR for healthcare, DORA for finance). 
*   **Action:** Read the relevant addendum to understand if your specific use cases trigger Annex III high-risk classifications or require prior Supervisory Authority consultation.

---

## Phase 3: Architect & Deploy (Days 45–90)

When the business demands a new, custom AI capability, IT must decide how to build it safely.

### Step 3.1: Choose the Deployment Architecture
*   **Tool:** [`templates/deployment-decision-matrix.md`](../templates/deployment-decision-matrix.md)
*   **Owner:** Chief Technology Officer (CTO) or Chief Architect.
*   **Why it matters:** Not every AI project needs a self-hosted Llama 3 model, and not every project is safe for the OpenAI public API. This matrix forces a structured decision based on data sensitivity and latency requirements.
*   **Action:** Require a completed decision matrix as part of the technical design document for any new AI initiative.

### Step 3.2: Conduct the Impact Assessment
*   **Tool:** [`templates/dpia-ai-template.md`](../templates/dpia-ai-template.md) (Reference the [`templates/dpia-example-library.md`](../templates/dpia-example-library.md) for guidance)
*   **Owner:** DPO & Product Owner.
*   **Why it matters:** GDPR Article 35 mandates a DPIA for processing that is "likely to result in a high risk," which almost all consequential AI systems do. The EU AI Act Article 27 also requires a Fundamental Rights Impact Assessment (FRIA) for certain high-risk deployers. This template combines both.
*   **Action:** Complete the DPIA *before* any code is written or data is processed.

### Step 3.3: Audit for Algorithmic Bias
*   **Tool:** [`guides/algorithmic-bias-audit-methodology.md`](algorithmic-bias-audit-methodology.md)
*   **Owner:** Lead Data Scientist & Compliance Officer.
*   **Why it matters:** If your system makes decisions about humans (credit, employment, housing), it will be scrutinized for bias. You must mathematically prove fairness.
*   **Action:** Follow the 4-phase methodology to select a fairness metric, test the model, and document the accuracy-fairness trade-off for the Annex IV technical documentation.

### Step 3.4: GPAI Governance (If Applicable)
*   **Tool:** [`templates/gpai-model-governance-checklist.md`](../templates/gpai-model-governance-checklist.md)
*   **Owner:** AI Engineering Lead.
*   **Why it matters:** If you are fine-tuning a General Purpose AI model or building one from scratch, you may trigger Article 53-55 obligations.
*   **Action:** Run the checklist to determine if you cross the 10^25 FLOPs systemic risk threshold and to ensure Annex XI/XII documentation is complete.

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
*   **Why it matters:** ISO/IEC 42001:2023 is the globally recognized standard for AI Management Systems. Achieving certification provides a presumption of conformity with many EU AI Act requirements.
*   **Action:** Use the 12-month roadmap to formalize your AI governance into a certifiable management system.

---

*This guide is part of the AI Compliance Framework by diShine Digital Agency.*

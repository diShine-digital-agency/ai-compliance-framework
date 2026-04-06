# Sector Addendum: Human Resources & Employment

**Version:** 1.2.0

The use of Artificial Intelligence in Human Resources (HR) is one of the most heavily regulated areas under the EU AI Act and the General Data Protection Regulation (GDPR). As of April 2026, the deployment of AI for recruitment, performance management, or termination decisions carries significant legal and reputational risks.

This addendum provides a pragmatic compliance framework for employers (deployers) and HR-tech vendors (providers).

---

## 1. The Regulatory Intersection (April 2026 Status)

The core complexity in HR AI is the intersection of the EU AI Act's high-risk classification, GDPR Article 22 (Automated Decision-Making), and the EU Employment Equality Directives.

*   **The Golden Rule:** If an AI system is intended to be used for recruitment, selection, or making decisions affecting terms of work, promotion, or termination, it is **automatically classified as a High-Risk AI System** under Annex III, Point 4 of the EU AI Act.
*   **The GDPR Article 22 Test:** GDPR prohibits decisions based *solely* on automated processing that produce legal or similarly significant effects on an individual. Hiring and firing are the textbook examples of "significant effects."
*   **The Indirect Discrimination Risk:** AI systems trained on historical HR data are highly susceptible to perpetuating historical biases, leading to indirect discrimination claims under EU equality law.

---

## 2. HR AI Risk Classification Matrix

Use this matrix to determine your regulatory burden based on the specific use case.

| Use Case | AI Act Class | GDPR Art. 22 | Equality Directive | Immediate Action Required |
| :--- | :--- | :--- | :--- | :--- |
| **CV Parsing & Automated Ranking** (e.g., scoring candidates 1-100) | 🔴 High-Risk (Annex III.4a) | Yes (If no human review) | High Risk (Bias) | Mandatory DPIA. Ensure a human reviews all rejected candidates before final decision. Document bias mitigation in training data. |
| **AI Video Interview Analysis** (e.g., analyzing tone, micro-expressions) | 🔴 High-Risk (Annex III.4a) | Yes | High Risk (Bias) | **Warning:** Emotion recognition in the workplace is generally prohibited (Art. 5). Ensure the tool only analyzes content, not emotion/biometrics. |
| **Performance Monitoring & Evaluation** (e.g., keystroke logging, sentiment analysis) | 🔴 High-Risk (Annex III.4b) | Yes (If tied to bonuses/firing) | Medium Risk | Mandatory DPIA. Consult Works Council/Employee Reps before deployment. Ensure transparency to workers (Art. 29). |
| **AI-Assisted Task Allocation** (e.g., algorithmic management of gig workers) | 🔴 High-Risk (Annex III.4b) | Yes | Medium Risk | Ensure human oversight (Art. 14) to override algorithmic assignments that are unfair or unsafe. |
| **Internal HR Chatbots** (e.g., answering policy questions) | 🟡 Limited Risk | No | Low Risk | Ensure clear transparency to employees that they are interacting with an AI (Art. 50). |

---

## 3. Key Compliance Requirements for High-Risk HR AI

If your system falls into the 🔴 High-Risk category above, you must implement the following controls:

### A. Meaningful Human Oversight (Article 14 & GDPR Art. 22)
The AI Act and GDPR explicitly forbid "rubber-stamping" AI decisions in HR.
*   **Action:** The AI system must be designed as a *decision support* tool, not a *decision-making* tool. A trained human HR professional must review the AI's recommendation (e.g., a candidate ranking) and have the authority and information necessary to override it. You must document this human review process.

### B. Bias Mitigation & Data Governance (Article 10)
HR data is inherently biased (e.g., historical preference for certain universities or demographics).
*   **Action:** Providers must proactively test their algorithms for disparate impact against protected characteristics (gender, race, age, disability). Deployers must ask vendors for their bias testing methodology and results before procurement.

### C. Transparency to Workers (Article 29)
Employees and candidates have a right to know when AI is evaluating them.
*   **Action:** Update privacy notices and employment contracts to explicitly state when and how AI is used for recruitment or performance management. Explain the logic involved in plain language.

### D. Prohibited Practices (Article 5)
The AI Act strictly prohibits certain uses of AI in the workplace.
*   **Action:** Ensure you are not using AI for **Emotion Recognition** (inferring emotions from facial expressions or voice) or **Social Scoring** (evaluating employees based on non-work-related social behavior).

---

## 4. Deployer vs. Provider Obligations

The regulatory burden shifts depending on your role:

*   **You are a PROVIDER if:** You develop the HR AI software (e.g., a startup building a CV screening tool). You bear the brunt of the AI Act: CE marking, technical documentation, QMS, and bias testing.
*   **You are a DEPLOYER if:** You use the HR AI software (e.g., a company buying the CV screening tool). Your obligations are:
    1.  Conduct a Fundamental Rights Impact Assessment (FRIA) / DPIA before deployment.
    2.  Ensure meaningful human oversight of the AI's outputs.
    3.  Inform candidates/employees that AI is being used.
    4.  Consult with Works Councils or employee representatives (mandatory in many EU jurisdictions like Germany and France).

*This addendum is part of the AI Compliance Framework by diShine Digital Agency.*

# Data Protection Impact Assessment (DPIA) for AI Systems

**Version:** 1.0
**Regulatory Context:** April 2026 (GDPR Article 35 & EU AI Act Alignment)

This template is specifically designed for conducting a DPIA on Artificial Intelligence systems. It goes beyond a standard IT DPIA by explicitly addressing AI-specific risks such as algorithmic bias, opacity ("black box" decision-making), and the complexities of model training data.

---

## Part 1: System Overview & Necessity

### 1.1 Project Details
*   **Project Name:** [Insert Name]
*   **Business Owner:** [Name/Title]
*   **Data Protection Officer (DPO):** [Name]
*   **AI System Provider (if third-party):** [Vendor Name]
*   **EU AI Act Risk Classification:** [Minimal / Limited / High-Risk (Annex III) / Prohibited]

### 1.2 Description of the Processing
*   **What is the AI system designed to do?** (e.g., "Automate initial CV screening for engineering roles.")
*   **What data is being processed?** (List all data categories. Highlight any Special Category Data under GDPR Art. 9, such as health data or biometric data.)
*   **Data Source:** (Where does the training data come from? Where does the operational input data come from?)
*   **Data Retention:** (How long is the input data stored? Is it used to further train the model?)

### 1.3 Necessity and Proportionality (GDPR Art. 35(7)(b))
*   **Why is AI necessary for this task?** (Could the same outcome be achieved with a simpler, non-AI rules-based system?)
*   **Is the data processing proportionate?** (Are you collecting more data than strictly necessary for the AI to function accurately?)

---

## Part 2: AI-Specific Risk Assessment

Assess the following risks to the rights and freedoms of data subjects. For each risk, assign a Likelihood (Low/Medium/High) and Severity (Low/Medium/High).

### 2.1 Algorithmic Bias and Discrimination
*   **Risk:** The AI model produces outputs that unfairly disadvantage specific groups (e.g., based on gender, race, age) due to biased training data or flawed model design.
*   **Likelihood:** [ ]
*   **Severity:** [ ]
*   **Mitigation Measures:** (e.g., "Training data was audited for demographic balance. Model outputs are statistically tested for disparate impact across protected classes monthly.")

### 2.2 Opacity and Lack of Explainability
*   **Risk:** The AI's decision-making process is a "black box," making it impossible to explain to a data subject *why* a specific decision was made about them (violating GDPR Art. 13-15 and Art. 22).
*   **Likelihood:** [ ]
*   **Severity:** [ ]
*   **Mitigation Measures:** (e.g., "We use interpretable models (e.g., decision trees) rather than deep neural networks for this specific task. We provide a 'reason code' alongside every AI output.")

### 2.3 Automated Decision-Making (GDPR Art. 22)
*   **Risk:** The system makes decisions based *solely* on automated processing that produce legal or similarly significant effects on the individual, without lawful basis or safeguards.
*   **Likelihood:** [ ]
*   **Severity:** [ ]
*   **Mitigation Measures:** (e.g., "The AI output is strictly advisory. A human reviewer makes the final decision. Data subjects have a clear UI path to request human intervention and contest the AI's recommendation.")

### 2.4 Data Leakage and Model Inversion
*   **Risk:** Sensitive personal data used in the training set can be extracted or inferred by users interacting with the operational AI model (e.g., via prompt injection or model inversion attacks).
*   **Likelihood:** [ ]
*   **Severity:** [ ]
*   **Mitigation Measures:** (e.g., "All training data is anonymized. The model is hosted in a private VPC with strict rate limiting and prompt filtering to prevent extraction attacks.")

---

## Part 3: Residual Risk & DPO Sign-Off

### 3.1 Residual Risk Assessment
After applying the mitigation measures in Part 2, what is the remaining level of risk?
*   **Overall Residual Risk:** [Low / Medium / High]

*(Note: If the residual risk remains HIGH despite mitigations, GDPR Article 36 requires you to consult your national Supervisory Authority before deploying the system.)*

### 3.2 DPO Advice and Sign-Off
*   **DPO Comments:** [Insert DPO analysis of the assessment and mitigations.]
*   **DPO Recommendation:** [Approve / Reject / Approve with Conditions]
*   **Signature & Date:** ___________________________

---
*This template is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

# DPIA Example Library: Pre-Filled AI Use Cases

**Version:** 1.2.0

Under GDPR Article 35 and the EU AI Act (Article 30 Fundamental Rights Impact Assessment), deploying high-risk AI systems requires a comprehensive Data Protection Impact Assessment (DPIA).

This library provides three pre-filled, pragmatic DPIA examples for common enterprise AI deployments. These are not generic templates; they contain specific risks, technical measures, and residual risk assessments based on April 2026 regulatory standards.

---

## Example 1: AI-Powered Recruitment Screening Tool

**System Name:** TalentMatch AI Recruitment Assistant
**Purpose:** Automate initial screening of job applications (CV parsing, skill extraction, candidate ranking) to improve efficiency and reduce human bias.

### 1. Data Flows & Categories
*   **Input Data:** Name, contact details, professional experience, education, skills, cover letter content. (Potential Special Category Data if voluntarily provided, e.g., disability status).
*   **Processed Data:** Extracted keywords, skill scores, inferred suitability rankings.
*   **Output Data:** Shortlisted candidate list, individual scores, rationale for ranking.
*   **Retention:** Unsuccessful candidates (6-12 months post-recruitment). Successful candidates (transferred to HR file).

### 2. Specific Risks & Impact Assessment
*   **Algorithmic Bias (GDPR Art. 5(1)(d), AI Act Art. 10):** Risk of perpetuating historical biases (e.g., gender, ethnicity) present in training data. *Impact:* Unfair treatment, discrimination claims, reputational damage.
*   **Lack of Transparency (GDPR Art. 13/14, AI Act Art. 13):** Candidates cannot understand how they were ranked or why they were rejected (the "black box" problem). *Impact:* Inability to exercise data subject rights, lack of trust.
*   **Automated Decision-Making (GDPR Art. 22):** System automatically rejecting candidates without human review. *Impact:* Violation of Art. 22(1), denial of employment opportunity based solely on automated processing.

### 3. Technical & Organisational Measures
*   **Bias Mitigation:** Vendor must provide evidence of diverse training data and continuous fairness audits against protected attributes.
*   **Transparency:** Inform candidates *prior* to application that AI is used for initial screening. Provide a clear explanation of the logic involved.
*   **Human Oversight (Mandatory):** The AI *assists* screening; it does not make final decisions. A trained HR professional reviews all shortlisted candidates and a sample of rejected candidates. A mechanism for human override is implemented.

### 4. Residual Risk Assessment
*   With mandatory human oversight and proactive bias testing, the residual risk of systemic discrimination is **Medium-Low**.
*   **DPO/SA Consultation:** Given the robust controls, prior consultation with the Supervisory Authority (GDPR Art. 36) is *not* triggered. However, the FRIA results must be documented internally.

---

## Example 2: AI Customer Service Chatbot with Sentiment Analysis

**System Name:** SupportBot Pro
**Purpose:** Handle tier-1 customer inquiries, analyze customer sentiment (frustration, anger) to prioritize routing to human agents, and summarize chat transcripts.

### 1. Data Flows & Categories
*   **Input Data:** Customer name, account ID, chat text, voice audio (if voicebot).
*   **Processed Data:** Intent classification, sentiment score (e.g., 0.8 Angry), entity extraction (e.g., product names).
*   **Output Data:** Automated responses, routing priority flags, chat summaries.
*   **Retention:** Chat transcripts retained for 90 days for quality assurance and model fine-tuning (if consent provided).

### 2. Specific Risks & Impact Assessment
*   **Special Category Data Inference (GDPR Art. 9):** Risk that sentiment analysis inadvertently infers health conditions (e.g., depression) or other protected characteristics from text/voice patterns. *Impact:* Unlawful processing of Art. 9 data without explicit consent.
*   **Data Minimisation Failures (GDPR Art. 5(1)(c)):** Chatbot ingesting and storing sensitive personal data (e.g., credit card numbers, passwords) typed by the customer in free-text fields. *Impact:* Increased risk of severe data breach.
*   **Lack of Transparency (AI Act Art. 50):** Customers believing they are interacting with a human. *Impact:* Violation of AI Act transparency obligations, erosion of trust.

### 3. Technical & Organisational Measures
*   **Data Masking:** Implement real-time Data Loss Prevention (DLP) to automatically redact PII/PCI data (e.g., credit cards, SSNs) from chat transcripts *before* they are processed by the NLP model or stored.
*   **Transparency:** The chatbot must explicitly state "I am an AI virtual assistant" at the beginning of every interaction.
*   **Sentiment Scope Limitation:** Restrict sentiment analysis strictly to customer service satisfaction (e.g., frustrated vs. satisfied). Prohibit the model from inferring deeper psychological states.

### 4. Residual Risk Assessment
*   With real-time DLP masking and strict scope limitations on sentiment analysis, the residual risk is **Low**.
*   **DPO/SA Consultation:** Not required.

---

## Example 3: AI-Powered Employee Performance Monitoring

**System Name:** WorkFlow Analytics AI
**Purpose:** Analyze employee digital activity (keystrokes, application usage, email metadata) to identify productivity bottlenecks, assess performance, and recommend training.

### 1. Data Flows & Categories
*   **Input Data:** Employee ID, active window titles, keystroke volume, email send/receive timestamps, calendar meeting density.
*   **Processed Data:** Productivity scores, focus time metrics, collaboration network graphs.
*   **Output Data:** Manager dashboards, individual performance reports, automated training recommendations.
*   **Retention:** Raw activity data aggregated daily and deleted after 30 days. Aggregated scores retained for annual review cycle.

### 2. Specific Risks & Impact Assessment
*   **Profiling & Power Imbalance (GDPR Art. 22):** High risk of profiling employees in a context of significant power imbalance. *Impact:* Chilling effect on employee behavior, stress, unfair performance evaluations based on flawed algorithmic assumptions (e.g., equating keystrokes with value).
*   **Lack of Legal Basis:** Consent is generally invalid in employment contexts due to power imbalance. Relying on Legitimate Interests (Art. 6(1)(f)) is highly contentious for pervasive monitoring. *Impact:* Unlawful processing, severe regulatory fines.
*   **Prohibited Practices (AI Act Art. 5):** Risk of crossing into prohibited "emotion recognition" if the system analyzes communication tone to infer employee morale or stress levels.

### 3. Technical & Organisational Measures
*   **Strict Anonymization/Aggregation:** The system must aggregate data at the team or department level (minimum 5 people) rather than individual level, unless strictly necessary and legally justified for a specific, documented performance issue.
*   **Works Council Consultation:** Mandatory consultation and agreement with employee representatives/Works Councils *prior* to procurement and deployment.
*   **Prohibit Automated Penalties:** The system output cannot be used to automatically trigger disciplinary action, bonus reduction, or termination. It must only be used as one data point in a holistic, human-led review.

### 4. Residual Risk Assessment
*   Even with aggregation, the inherent risks of workplace monitoring are high. The residual risk remains **High**.
*   **DPO/SA Consultation:** A DPIA is mandatory. Depending on national law (e.g., Germany, France) and the specific intrusiveness of the tool, **Prior Consultation with the Supervisory Authority (GDPR Art. 36) is highly likely to be triggered** before deployment.

*This library is part of the AI Compliance Framework by diShine Digital Agency.*

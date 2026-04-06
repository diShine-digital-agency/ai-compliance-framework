# Sector Addendum: Healthcare & Life Sciences

**Version:** 1.2.0

The healthcare sector faces the most stringent intersection of AI regulation globally. As of April 2026, deploying AI in clinical or administrative healthcare settings requires navigating the EU AI Act, the Medical Device Regulation (MDR 2017/745), the In Vitro Diagnostic Regulation (IVDR 2017/746), and GDPR Article 9 (Special Category Data).

This addendum provides a pragmatic compliance framework for healthcare providers (deployers) and health-tech vendors (providers).

---

## 1. The Regulatory Intersection (April 2026 Status)

The core complexity in healthcare AI is the overlap between medical device law and AI law.

*   **The Golden Rule:** If an AI system qualifies as a Medical Device under MDR Article 2(1) or an IVD under IVDR Article 2(1), it is **automatically classified as a High-Risk AI System** under Annex III, Point 5 of the EU AI Act.
*   **The Intended Purpose Test:** Classification hinges entirely on the manufacturer's stated *intended purpose*. If the software claims to diagnose, prevent, monitor, predict, prognosticate, treat, or alleviate disease, it is a medical device.
*   **Administrative vs. Clinical:** AI used for hospital bed scheduling or billing is generally *not* a medical device and may only be subject to GDPR and general AI Act transparency rules. AI used for Clinical Decision Support Systems (CDSS) is almost always high-risk.

---

## 2. Healthcare AI Risk Classification Matrix

Use this matrix to determine your regulatory burden based on the specific use case.

| Use Case | AI Act Class | MDR/IVDR Status | GDPR Art. 9 | Immediate Action Required |
| :--- | :--- | :--- | :--- | :--- |
| **Diagnostic Imaging Analysis** (e.g., detecting tumors in MRIs) | 🔴 High-Risk (Annex III.5) | Yes (Class IIa or higher) | Yes (Health Data) | Full QMS (ISO 13485 + ISO 42001), Notified Body conformity assessment, mandatory DPIA. |
| **Clinical Decision Support (CDSS)** (e.g., sepsis prediction algorithms) | 🔴 High-Risk (Annex III.5) | Yes (Class IIa or higher) | Yes (Health Data) | Implement strict "Human-in-the-loop" oversight (Art. 14). Document clinical validation data. |
| **AI-Powered Triage Chatbots** (e.g., symptom checkers directing patients) | 🔴 High-Risk (Annex III.5) | Yes (Class I or IIa) | Yes (Health Data) | Ensure clear transparency to patients that they are interacting with AI (Art. 50). |
| **Medical Transcription / Ambient Scribes** (e.g., converting speech to clinical notes) | 🟡 Limited Risk | No (Usually) | Yes (Health Data) | Focus on GDPR compliance (consent or Art. 9(2)(h) exception). Ensure data is not used for vendor model training without explicit consent. |
| **Hospital Resource Optimization** (e.g., predicting bed availability) | 🟢 Minimal Risk | No | No (If anonymized) | Standard IT procurement checks. Ensure data anonymization protocols are robust. |

---

## 3. Key Compliance Requirements for High-Risk Healthcare AI

If your system falls into the 🔴 High-Risk category above, you must implement the following controls:

### A. Data Governance & Bias Mitigation (Article 10)
Healthcare data is notoriously biased (e.g., pulse oximeters performing poorly on darker skin tones). The AI Act requires proactive bias mitigation.
*   **Action:** Document the demographic breakdown of your training, validation, and testing datasets. Prove that the data is relevant, representative, and free of errors that could lead to discriminatory health outcomes.

### B. Human Oversight (Article 14)
The AI Act explicitly forbids "automation bias" (humans blindly trusting the machine) in high-risk scenarios.
*   **Action:** Design the UI/UX of the CDSS so that the clinician is forced to actively review the AI's recommendation. The system must provide a confidence score or rationale (Explainable AI) to allow the clinician to make an informed final decision.

### C. GDPR Article 9 Exceptions
Processing health data is generally prohibited unless an exception applies.
*   **Action:** For clinical care, rely on **Article 9(2)(h)** (provision of health or social care). For training AI models, you generally cannot rely on 9(2)(h); you must obtain **Explicit Consent (Article 9(2)(a))** or rely on **Scientific Research (Article 9(2)(j))** with robust pseudonymization/anonymization safeguards.

---

## 4. Deployer vs. Provider Obligations

The regulatory burden shifts depending on your role:

*   **You are a PROVIDER if:** You develop the AI system (e.g., a health-tech startup building a radiology AI). You bear the brunt of the AI Act: CE marking, technical documentation, QMS, and post-market monitoring.
*   **You are a DEPLOYER if:** You use the AI system (e.g., a hospital buying the radiology AI). Your obligations are:
    1.  Use the system strictly according to the provider's instructions.
    2.  Ensure human oversight is actually performed by competent medical staff.
    3.  Monitor for anomalies and report incidents to the provider and authorities.
    4.  Conduct a Fundamental Rights Impact Assessment (FRIA) / DPIA before deployment.

*This addendum is part of the AI Compliance Framework by diShine Digital Agency.*

# AI Incident Response Playbook

**Version:** 1.3.0

Traditional cybersecurity incident response plans (IRPs) are insufficient for Artificial Intelligence. When an AI system fails, it rarely looks like a traditional hack; it looks like a model hallucinating sensitive data, a silent degradation in accuracy, or an algorithmic bias that triggers a regulatory investigation.

This playbook provides a structured, forensic approach to AI incident response, aligned with the **EU AI Act (Article 73)**, **GDPR (Article 33/34)**, and the **NIST AI Risk Management Framework (AI RMF 1.0)**.

---

## 1. Incident Classification Taxonomy

Not all AI anomalies are incidents. Use this taxonomy to classify events and trigger the appropriate response tier.

| Severity | Definition | Examples | Response SLA |
| :--- | :--- | :--- | :--- |
| **P1: Critical** | Severe harm to health/safety, fundamental rights breach, or massive data leak. Triggers EU AI Act Art. 73 "Serious Incident". | CDSS recommends lethal drug dose; LLM leaks thousands of PII records; Autonomous system causes physical injury. | **Immediate (1 hour)** |
| **P2: High** | Significant financial loss, regulatory violation (GDPR), or widespread algorithmic bias affecting a protected class. | HR AI systematically rejects female candidates; Financial AI causes flash crash; Prompt injection bypasses all safety filters. | **4 Hours** |
| **P3: Medium** | Model drift exceeding acceptable thresholds, localized data poisoning, or non-critical hallucinations. | Customer service bot invents a fake refund policy; 10% drop in model accuracy over 1 week. | **24 Hours** |
| **P4: Low** | Minor anomalies, isolated user complaints about AI output, or scheduled maintenance issues. | Single user reports a weird chatbot response; minor latency in API calls. | **Next Business Day** |

---

## 2. The 6-Phase AI Incident Response Lifecycle

### Phase 1: Preparation & Governance (NIST GOVERN/MAP)
*   **Establish the AI-IRT:** Form an AI Incident Response Team including Data Science, Legal/Compliance, IT Security, and PR.
*   **Logging & Telemetry:** Ensure all high-risk AI systems have immutable logging enabled (EU AI Act Art. 12). You cannot investigate an AI incident without input/output logs and model version history.
*   **Kill Switches:** Implement automated circuit breakers and manual kill switches for all production models.

### Phase 2: Detection & Triage (NIST MEASURE)
*   **Monitoring Triggers:** Set alerts for statistical deviation (model drift), sudden spikes in API error rates, or specific keyword triggers in LLM outputs (e.g., profanity, competitor names).
*   **Triage Questions:**
    1. Is the model producing harmful, biased, or factually dangerous outputs?
    2. Has personal data (PII) or intellectual property (IP) been exposed?
    3. Is the system under active adversarial attack (e.g., prompt injection, data poisoning)?

### Phase 3: Containment & Mitigation (NIST MANAGE)
*   **Tier 1 Containment (Soft):** Route all AI traffic to a human fallback (Human-in-the-loop) or a simpler, deterministic rules engine.
*   **Tier 2 Containment (Hard):** Activate the kill switch. Take the model offline immediately.
*   **Evidence Preservation:** **DO NOT OVERWRITE THE MODEL.** Preserve the exact model weights, the specific training data snapshot, and the inference logs from the time of the incident. This is critical for forensic analysis and regulatory reporting.

### Phase 4: Forensic Investigation & Root Cause Analysis
Determine the exact nature of the failure:
*   **Data Poisoning:** Was the training or fine-tuning data intentionally corrupted?
*   **Adversarial Attack:** Did a user employ prompt injection, jailbreaking, or model inversion techniques?
*   **Model Drift / Concept Drift:** Did the real-world data change so much that the model's underlying assumptions are no longer valid?
*   **Hallucination / Stochastic Failure:** Did the LLM simply generate a statistically probable but factually incorrect output?

### Phase 5: Regulatory Notification & Communication
*   **EU AI Act (Article 73):** If P1 (Serious Incident), notify the national Market Surveillance Authority (MSA) **within 15 days**. If it involves death or widespread infringement, notify within **2 to 10 days**.
*   **GDPR (Article 33/34):** If the AI incident resulted in a personal data breach (e.g., model inversion revealing PII), notify the Data Protection Authority (DPA) **within 72 hours**.
*   **Internal/External Comms:** Draft communications explaining the AI failure without using overly technical jargon. Be transparent about the steps taken to fix the model.

### Phase 6: Recovery & Post-Incident Review
*   **Model Retraining:** Retrain the model with corrected data, updated safety filters, or improved adversarial robustness.
*   **Validation:** Run the model through a rigorous red-teaming exercise before redeployment.
*   **Documentation:** Update the AI system's Technical Documentation (EU AI Act Annex XI) with the incident details and the corrective actions taken.

---

## 3. Specific AI Attack Vectors & Response Tactics

### A. Prompt Injection / Jailbreaking
*   **Symptoms:** LLM ignores system prompts, outputs restricted information, or executes unauthorized commands.
*   **Response:** Immediately update input validation filters. Review system prompt architecture to separate instructions from user data.

### B. Model Inversion / Data Extraction
*   **Symptoms:** Attackers successfully query the model to reveal sensitive training data (e.g., extracting SSNs from a healthcare LLM).
*   **Response:** Treat as a severe Data Breach (GDPR Art. 33). Take the model offline. Implement differential privacy techniques or stricter output filtering before redeployment.

### C. Algorithmic Bias Discovery
*   **Symptoms:** Internal audit or external complaint reveals the model is systematically discriminating against a protected class.
*   **Response:** Suspend automated decision-making. Revert to manual human review. Conduct a full fairness audit on the training data and model weights.

*This playbook is part of the AI Compliance Framework by diShine Digital Agency.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 4 — Monitor & Respond**, **Step 4.1: Prepare for Incidents**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

# General Purpose AI (GPAI) Model Governance Checklist

**Version:** 1.3.0

Under the EU AI Act, General Purpose AI (GPAI) models—such as large language models (LLMs) and foundation models—are subject to specific obligations under Articles 53 to 55. These rules apply to the *models* themselves, distinct from the *systems* they are integrated into.

This checklist is designed for organizations that **develop**, **fine-tune**, or **deploy** GPAI models. It reflects the regulatory landscape as of April 2026, including the final GPAI Code of Practice.

---

## 1. Determine Your Role & Scope

Before applying the checklist, you must determine your legal role under the AI Act.

*   **Are you a Provider?** You are a provider if you develop a GPAI model (e.g., training a new foundation model from scratch) or if you substantially modify an existing GPAI model (e.g., fine-tuning an open-source model like Llama 3 on proprietary data to the extent that its core capabilities change).
*   **Are you a Deployer?** You are a deployer if you use a GPAI model via an API (e.g., building an app on top of OpenAI's GPT-4) without modifying the underlying model weights.
*   **Is the model "Systemic Risk"?** A GPAI model is presumed to have systemic risk if it was trained using a total computing power exceeding **10^25 FLOPs** (Article 51). The European AI Office can also designate models as systemic based on other criteria (e.g., reach, capability).

---

## 2. Baseline Obligations for ALL GPAI Providers (Article 53)

If you are a Provider of *any* GPAI model (even non-systemic), you must comply with Article 53.

### A. Technical Documentation (Annex XI)
*   [ ] **Model Description:** Document the model's architecture, parameter count, modalities (text, image, audio), and intended tasks.
*   [ ] **Development Process:** Detail the training methodology, optimization techniques, and internal evaluation results.
*   [ ] **Compute & Energy:** Estimate the total compute resources used (in FLOPs) and the energy consumed during training.
*   [ ] **Retention:** Ensure this documentation is kept up-to-date and retained for 10 years after the model is placed on the market.

### B. Downstream Provider Information (Annex XII)
*   [ ] **Capabilities & Limitations:** Provide clear documentation to downstream developers detailing what the model can do, its known limitations, and circumstances where performance degrades.
*   [ ] **Safety Performance:** Disclose known hazards, failure modes, and the results of safety evaluations.
*   [ ] **Acceptable Use:** Clearly state the intended uses and explicitly exclude prohibited uses.

### C. Copyright Compliance & Training Data Transparency
*   [ ] **Copyright Policy:** Implement a policy to respect EU copyright law, specifically the text and data mining (TDM) opt-outs under the DSM Directive (Article 4(3)).
*   [ ] **Data Summary:** Publish a sufficiently detailed summary of the training data using the mandatory template provided by the AI Office. This must include data modalities, approximate dataset size, and data provenance.

---

## 3. Additional Obligations for SYSTEMIC RISK GPAI Providers (Article 55)

If your model exceeds the 10^25 FLOPs threshold or is otherwise designated as having systemic risk, you must comply with Article 55 in addition to Article 53.

### A. Model Evaluation & Adversarial Testing
*   [ ] **Standardized Evaluation:** Perform rigorous model evaluations using state-of-the-art protocols and tools to identify and mitigate systemic risks.
*   [ ] **Red-Teaming:** Conduct adversarial testing (red-teaming) to probe the model for vulnerabilities, safety flaws, and potential for misuse (e.g., generating biological weapons instructions, bypassing safety filters). Document the methodology and results.

### B. Incident Reporting & Cybersecurity
*   [ ] **Incident Tracking:** Track and report serious incidents and possible systemic risks to the AI Office and relevant national authorities without undue delay.
*   [ ] **Cybersecurity:** Ensure an adequate level of cybersecurity protection for the model and its physical infrastructure (e.g., protecting model weights from theft or unauthorized access).

---

## 4. Obligations for GPAI Deployers (API Users)

If you are building an application on top of a third-party GPAI model (e.g., using an API), your primary obligations relate to the *system* you are building, not the underlying model.

*   [ ] **Vendor Due Diligence:** Verify that the GPAI provider (e.g., OpenAI, Anthropic) complies with Article 53 (and Article 55 if applicable). Request their Annex XII downstream documentation.
*   [ ] **System Classification:** Determine if your specific application (the AI system) falls under Annex III High-Risk categories (e.g., using the API for recruitment screening or medical diagnosis). If yes, you bear the full compliance burden for the high-risk system.
*   [ ] **Transparency (Article 50):** If your system interacts directly with natural persons (e.g., a chatbot), you must inform them that they are interacting with an AI system.

---

## 5. The GPAI Code of Practice (Voluntary Compliance)

The European Commission published the final General-Purpose AI Code of Practice in July 2025.

*   [ ] **Signatory Status:** Consider voluntarily signing the Code of Practice. The AI Office and AI Board have confirmed that adherence to the Code is an adequate means of demonstrating compliance with the AI Act's GPAI obligations.
*   [ ] **Implementation:** Review the specific chapters of the Code (Transparency, Copyright, Safety and Security) and implement the recommended state-of-the-art practices.

*This checklist is part of the AI Compliance Framework by diShine Digital Agency.*

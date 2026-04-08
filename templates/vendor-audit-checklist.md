# AI Vendor Audit Checklist (GDPR & EU AI Act)

**Version:** 1.0
**Auditor:** [Name/Role]
**Vendor Name:** [Vendor]
**Date:** [Date]

This checklist is designed to evaluate third-party AI vendors (SaaS, APIs, or integrated tools) against the stringent requirements of the **EU AI Act** and the **GDPR**. High-risk AI system obligations under Annex III apply from **2 December 2027** (as revised by the Digital Omnibus); transparency obligations under Article 50 apply from **2 November 2026**.

It goes beyond standard SOC 2 or ISO 27001 questionnaires to address the unique risks of Large Language Models (LLMs) and Generative AI.

---

## Part 1: Data Processing & GDPR Compliance

### 1.1 Data Usage for Model Training
*The most critical question for any enterprise AI deployment.*
- [ ] **Does the vendor explicitly state in their Data Processing Agreement (DPA) or Terms of Service that customer data (prompts, inputs, files) is NOT used to train their foundational models?**
- [ ] If they do use data for training, is there a clear, enterprise-wide opt-out mechanism that is enabled by default?
- [ ] Does the vendor use customer data to improve "service quality" (which often means fine-tuning smaller models)? If so, can this be disabled?

### 1.2 Data Retention & Deletion
*AI APIs often retain data for abuse monitoring.*
- [ ] What is the exact retention period for data submitted via the API or user interface? (e.g., OpenAI API retains for 30 days).
- [ ] Can the retention period be configured to zero (immediate deletion after processing)?
- [ ] Are there mechanisms for the customer to trigger immediate deletion of specific data points (Right to Erasure)?

### 1.3 Data Residency & Cross-Border Transfers
*Crucial for EU companies using US-based AI providers.*
- [ ] Where is the data physically processed and stored during inference (when the model generates a response)?
- [ ] Does the vendor offer EU-only data residency options (e.g., Azure OpenAI in European regions)?
- [ ] If data is transferred outside the EEA, are valid Standard Contractual Clauses (SCCs) or an Adequacy Decision in place? *Note: The EU-US Data Privacy Framework (DPF) was upheld by the EU General Court in September 2025 (Latombe case), but remains under legal uncertainty — a "Schrems III" challenge is anticipated. **Always implement SCCs as a parallel safeguard** alongside the DPF to ensure continuity if the adequacy decision is invalidated.*

### 1.4 Automated Decision-Making (Article 22)
*If the AI tool is used for HR, credit scoring, or profiling.*
- [ ] Does the tool make decisions that produce legal effects or similarly significantly affect individuals?
- [ ] If yes, does the vendor provide the necessary transparency and mechanisms for human intervention/review?
- [ ] Does the vendor provide sufficient documentation to allow the customer to conduct a Data Protection Impact Assessment (DPIA)?

---

## Part 2: EU AI Act Compliance

### 2.1 Risk Classification
*Determining the regulatory burden.*
- [ ] Has the vendor formally classified their AI system under the EU AI Act (Unacceptable, High-Risk, Limited Risk, Minimal Risk)?
- [ ] If the tool is used for Employment/HR, Critical Infrastructure, or Biometrics, it is likely **High-Risk** (Annex III). Does the vendor acknowledge this?

### 2.2 High-Risk System Obligations (If Applicable)
*If the vendor provides a High-Risk system, they must comply with Title III, Chapter 2.*
- [ ] **Risk Management System (Article 9):** Does the vendor have a documented, continuous risk management system for the AI tool?
- [ ] **Data Governance (Article 10):** Can the vendor prove the training data was relevant, representative, and free of errors/biases?
- [ ] **Technical Documentation (Article 11):** Is comprehensive technical documentation available to the customer (the "deployer") before deployment?
- [ ] **Human Oversight (Article 14):** Does the tool's design allow for effective human oversight by the customer's employees?
- [ ] **Accuracy & Cybersecurity (Article 15):** What are the vendor's documented metrics for accuracy, robustness, and cybersecurity against adversarial attacks (e.g., prompt injection)?

### 2.3 General-Purpose AI (GPAI) Obligations (If Applicable)
*If the vendor provides a foundational model (e.g., OpenAI, Anthropic).*
- [ ] **Copyright Policy (Article 53):** Does the vendor have a policy to comply with EU copyright law regarding their training data?
- [ ] **Training Data Summary:** Has the vendor published a sufficiently detailed summary of the content used for training the GPAI model?
- [ ] **Systemic Risk:** Has the model been designated as having "systemic risk"? If so, what additional mitigations are in place?

### 2.4 Transparency Obligations (Limited Risk)
*For chatbots, deepfakes, and emotion recognition.*
- [ ] If the tool is a chatbot or virtual assistant, does it clearly inform the end-user that they are interacting with an AI system (Article 50)?

---

## Part 3: Security & Intellectual Property

### 3.1 Prompt Security & Isolation
- [ ] Are customer prompts and generated outputs logically isolated from other customers in a multi-tenant environment?
- [ ] Does the vendor offer dedicated instances or Virtual Private Cloud (VPC) deployments for enhanced isolation?

### 3.2 Intellectual Property Rights
- [ ] Does the vendor explicitly assign all Intellectual Property rights of the *generated output* to the customer?
- [ ] Does the vendor claim any ownership or license over the *input prompts* provided by the customer?

### 3.3 Sub-processors
- [ ] Does the vendor use third-party LLMs (e.g., a SaaS tool that uses OpenAI's API on the backend)?
- [ ] If yes, are those sub-processors listed in the DPA, and do they adhere to the same strict data non-training and retention policies?

---
*This checklist is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework. It is a starting point for vendor due diligence and should be adapted to your specific industry regulations.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 2 — Audit & Procure**, **Step 2.1: Audit Existing Vendors**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

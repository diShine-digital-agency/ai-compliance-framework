# AI Compliance Framework: Technology Sector Addendum

**Version:** 1.0
**Regulatory Context:** April 2026

This addendum extends the core AI Compliance Framework for organizations operating in the Technology sector (SaaS vendors, AI product builders, cloud providers). It maps the core templates to sector-specific regulations including the EU AI Act (Provider vs. Deployer roles), NIS2, and the Cyber Resilience Act (CRA).

---

## 1. The Critical Distinction: Provider vs. Deployer

The EU AI Act (Regulation 2024/1689) assigns obligations based on your role in the AI value chain. A single Tech company often holds multiple roles simultaneously.

| Role | Definition | Key Obligations |
| :--- | :--- | :--- |
| **Provider** | You build and sell an AI product under your own brand (even if built on a foundational model like OpenAI). | Maximum burden. If the system is High-Risk (Annex III), you must conduct conformity assessments, register in the EU database, and maintain a full Quality Management System (QMS). |
| **Deployer** | You use an AI system internally (e.g., an off-the-shelf AI HR tool for your own hiring). | Must ensure human oversight, monitor for anomalies, keep logs, and conduct a DPIA if required by GDPR. |
| **Distributor** | You resell or provide a marketplace for third-party AI tools. | Must verify the Provider has affixed the CE mark and provided required documentation. |

*Action Item:* Use the `deployment-decision-matrix.md` not just for infrastructure, but to explicitly document your legal role for every AI system in your stack.

---

## 2. Building on Foundational Models (GPAI)

If your SaaS product is a "wrapper" or built on top of a General-Purpose AI (GPAI) model (e.g., using the GPT-4 API):

*   **You are the Provider of the downstream system.**
*   The creator of the foundational model (e.g., OpenAI) is responsible for Article 53 GPAI obligations (copyright policy, training data summaries).
*   **Your Obligation:** You must perform due diligence to ensure the GPAI model you selected is suitable for your specific use case, especially if your downstream application is classified as High-Risk. You cannot simply pass all liability upstream.

---

## 3. When Does a SaaS Product Become "High-Risk"?

Most B2B SaaS AI features (e.g., text summarization, code generation, basic analytics) are **Minimal Risk**. However, your product becomes **High-Risk (Annex III)** if it touches specific domains:

*   **HR Tech & Recruitment:** AI used for screening CVs, evaluating candidates, or monitoring employee performance (Annex III, Point 4).
*   **EdTech:** AI used for grading exams or determining admissions (Annex III, Point 3).
*   **Biometrics:** Any system using biometric categorization or emotion recognition (Annex III, Point 1).
*   **Critical Infrastructure:** AI managing network traffic or cybersecurity for essential services (Annex III, Point 2).

*Action Item:* If your product falls into these categories, the `acceptable-use-policy.md` is insufficient. You must implement a full ISO 42001-aligned AI Management System.

---

## 4. Intersection with NIS2 and the Cyber Resilience Act (CRA)

*   **NIS2 Directive:** If your company is an "essential" or "important" entity (e.g., a cloud provider or managed service provider), your AI systems are part of your critical digital infrastructure. You must report significant AI-related cybersecurity incidents within 24 hours.
*   **Cyber Resilience Act (CRA):** AI-powered software products are "products with digital elements." You must ensure "Security by Design," handle vulnerabilities throughout the product lifecycle, and affix a CE mark demonstrating cybersecurity conformity, *in addition* to AI Act conformity.

---

## 5. Article 50 Transparency Obligations

If your SaaS product includes a chatbot, virtual assistant, or generates deepfakes:

*   **Chatbots:** You must explicitly inform users they are interacting with an AI (unless it is glaringly obvious from the context).
*   **Deepfakes/AI Content:** AI-generated audio, video, or image content must be clearly labeled in a machine-readable format (e.g., C2PA metadata) to indicate it is artificially generated or manipulated.

---

## 6. Immediate Action Plan (April 2026)

1.  **Role Mapping:** Document whether you are a Provider, Deployer, or Distributor for every AI system you build, buy, or sell.
2.  **Annex III Audit:** Review your product roadmap against Annex III of the EU AI Act. If you are building a High-Risk system, halt deployment until a conformity assessment plan is in place.
3.  **Implement Transparency:** Ensure all customer-facing chatbots and AI-generated content features have explicit, user-visible disclosures to comply with Article 50.

---
*This addendum is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 2 — Audit & Procure**, **Step 2.2: Map Sector-Specific Obligations**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](../guides/how-to-use-this-framework.md).

# Acceptable AI Use Policy

**Version:** 1.0
**Effective Date:** [Date]
**Owner:** [CISO / Legal / IT Director]

## 1. Purpose and Scope

This policy establishes the acceptable use of Artificial Intelligence (AI) tools, including Generative AI (GenAI) and Large Language Models (LLMs), by employees, contractors, and third parties acting on behalf of **[Company Name]**. 

The purpose is to harness the productivity benefits of AI while strictly mitigating risks related to:
- **Intellectual Property (IP) Leakage:** Inadvertent disclosure of trade secrets or proprietary code (e.g., the 2023 Samsung ChatGPT incident).
- **Data Privacy (GDPR):** Unauthorized processing of Personally Identifiable Information (PII).
- **Regulatory Compliance (EU AI Act):** Ensuring [Company Name] does not inadvertently deploy prohibited or high-risk AI systems without proper governance.
- **Shadow AI:** The unsanctioned use of consumer-grade AI tools that bypass IT security controls.

## 2. Approved vs. Prohibited AI Tools

### 2.1 Approved Enterprise AI Tools
Only AI tools that have undergone a formal security and legal review, and for which [Company Name] has a signed Data Processing Agreement (DPA) ensuring data is **not used to train the provider's foundational models**, are approved for business use.

**Current Approved Tools:**
- [e.g., Microsoft Copilot for Enterprise]
- [e.g., OpenAI API (Enterprise Tier Only)]
- [e.g., Internal Custom LLM deployed in VPC]

### 2.2 Prohibited Consumer AI Tools (Shadow AI)
The use of consumer-grade, free, or individual-subscription AI tools for company business is **strictly prohibited**. These tools often retain prompt history and may use input data for model training, violating our confidentiality obligations.

**Examples of Prohibited Tools for Company Data:**
- ChatGPT (Free or Plus tiers)
- Claude.ai (Free or Pro tiers)
- Google Gemini (Consumer web interface)
- Any unauthorized browser extensions or plugins claiming AI capabilities.

## 3. Data Classification and AI Input Rules

Employees must adhere to [Company Name]'s existing Data Classification Policy when interacting with *Approved* AI tools.

| Data Classification | Definition | Permitted in Approved AI Tools? | Permitted in Prohibited AI Tools? |
| :--- | :--- | :--- | :--- |
| **Public** | Information already available to the general public (e.g., published marketing copy, press releases). | **YES** | **YES** (with caution) |
| **Internal** | Routine business communications, non-sensitive operational data. | **YES** | **NO** |
| **Confidential** | PII, financial data, unreleased product roadmaps, strategic plans. | **RESTRICTED** (Requires specific IT/Legal approval per use case) | **NO** |
| **Restricted / Secret** | Source code, trade secrets, highly sensitive PHI/financials, M&A data. | **NO** (Unless using a fully air-gapped, self-hosted internal model) | **NO** |

## 4. Specific Prohibitions and Guidelines

### 4.1 Intellectual Property and Source Code
Employees must **never** input unredacted proprietary source code, algorithms, or architectural designs into any external AI tool, even approved ones, unless explicitly authorized by the CTO. Doing so may constitute a legal disclosure of trade secrets, voiding IP protections.

### 4.2 Personal Data (GDPR Compliance)
Employees must **never** input Personally Identifiable Information (PII) belonging to customers, employees, or partners into any AI tool without explicit authorization from the Data Protection Officer (DPO). This includes names, emails, addresses, or any data that could identify an individual.

### 4.3 Output Verification (Hallucinations)
AI models are prone to "hallucinations" (generating false or fabricated information). Employees are solely responsible for the accuracy, legality, and appropriateness of any work product generated with the assistance of AI. **All AI-generated output must be fact-checked and reviewed by a human before being used in any official capacity, published, or sent to clients.**

### 4.4 Automated Decision-Making (Article 22)
Employees must not use AI tools to make automated decisions that produce legal effects concerning individuals or similarly significantly affect them (e.g., automated resume screening, credit scoring, performance evaluations) without explicit legal review and the implementation of mandatory human oversight.

## 5. Reporting and Enforcement

### 5.1 Reporting Suspected Leaks
If an employee suspects that Confidential or Restricted data has been inadvertently entered into an unauthorized AI tool, they must immediately report the incident to [IT Security / Incident Response Team] at [Email/Phone]. **Do not attempt to delete the chat history before IT has investigated.**

### 5.2 Enforcement
Violations of this policy, particularly the intentional use of Shadow AI for sensitive data or the input of Restricted IP into external models, may result in disciplinary action up to and including termination of employment.

---
*This template is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework. It should be reviewed by your legal counsel before implementation.*

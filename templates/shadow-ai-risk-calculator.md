# Shadow AI Risk Calculator

**Version:** 1.0

This self-assessment tool helps organizations quantify their exposure to Shadow AI — the use of AI tools by employees without IT oversight. It is based on documented risk factors from the IBM Cost of a Data Breach 2024 Report, Gartner's 2025 Shadow AI predictions, and XM Cyber's enterprise AI research.

**How to use it:** Answer each question honestly. Add up your score. The result maps to a risk band with specific remediation priorities.

---

## Section A: Organizational Awareness (Max 25 points)

| # | Question | 0 points | 5 points |
| :--- | :--- | :--- | :--- |
| A1 | Does your company have a formal, written AI Use Policy? | No | Yes |
| A2 | Have employees received training on AI data risks in the last 12 months? | No | Yes |
| A3 | Do employees know which AI tools are officially approved? | No | Yes |
| A4 | Does your IT team have visibility into which AI tools are being used on company devices? | No | Yes |
| A5 | Is there a clear process for employees to report accidental data exposure via AI tools? | No | Yes |

**Section A Score: _____ / 25**

---

## Section B: Technical Controls (Max 30 points)

| # | Question | 0 points | 5 points | 10 points |
| :--- | :--- | :--- | :--- | :--- |
| B1 | What is the primary AI deployment tier used for business-critical workflows? | Tier 1 (Consumer APIs) | Tier 2 (Enterprise API) | Tier 3/4 (Private/Self-hosted) |
| B2 | Are signed Data Processing Agreements (DPAs) in place with all AI vendors? | No | Partially | Yes, for all vendors |
| B3 | Is there network-level blocking of unauthorized AI services (e.g., via DNS filtering or proxy)? | No | Partially | Yes |

**Section B Score: _____ / 30**

---

## Section C: Data Governance (Max 25 points)

| # | Question | 0 points | 5 points |
| :--- | :--- | :--- | :--- |
| C1 | Does your company have a formal Data Classification Policy (Public / Internal / Confidential / Restricted)? | No | Yes |
| C2 | Are employees trained on which data classification levels are prohibited from AI tools? | No | Yes |
| C3 | Has a Data Protection Impact Assessment (DPIA) been conducted for any AI-powered workflows? | No | Yes |
| C4 | Is there a process for auditing what data has been submitted to AI tools in the last 90 days? | No | Yes |
| C5 | Do all AI vendor contracts explicitly state that customer data is not used for model training? | No | Yes |

**Section C Score: _____ / 25**

---

## Section D: Incident History (Max 20 points)

| # | Question | 0 points | 10 points | 20 points |
| :--- | :--- | :--- | :--- | :--- |
| D1 | Has your organization experienced a known or suspected AI-related data incident in the last 24 months? | Yes, confirmed | Suspected but unconfirmed | No known incidents |
| D2 | Have any employees been disciplined or warned for using unauthorized AI tools with company data? | Yes, multiple cases | Yes, isolated case | No known cases |

**Section D Score: _____ / 20**

---

## Total Score and Risk Band

Add up your scores from all four sections.

**Total Score: _____ / 100**

| Score Range | Risk Band | Interpretation | Immediate Priority |
| :---: | :--- | :--- | :--- |
| **85 – 100** | 🟢 **Managed** | Strong controls in place. Focus on continuous improvement and monitoring. | Conduct quarterly audits; keep policies updated with regulatory changes. |
| **65 – 84** | 🟡 **Moderate** | Foundational controls exist but gaps remain. A single incident could escalate quickly. | Close the specific gaps identified in your lowest-scoring section. |
| **40 – 64** | 🟠 **Elevated** | Significant exposure. Employees are likely using unauthorized AI tools with company data today. | Immediately implement a formal AI Use Policy and deploy network-level blocking. |
| **0 – 39** | 🔴 **Critical** | High probability of an active Shadow AI incident. IBM data suggests breaches tied to Shadow AI add an average of **$670,000** to the total breach cost. | Treat as an active security incident. Conduct a full AI tool audit before proceeding. |

---

## Remediation Roadmap by Risk Band

### 🔴 Critical (0–39): Immediate Actions
1. Conduct an emergency audit of all AI tools currently in use across the organization (survey employees anonymously if needed);
2. Issue an immediate communication to all employees clarifying that consumer AI tools (ChatGPT Plus, Claude Pro, etc.) must not be used for any company data;
3. Engage legal counsel to assess whether any existing incidents constitute a GDPR data breach requiring notification to the supervisory authority within 72 hours (Article 33).

### 🟠 Elevated (40–64): 30-Day Sprint
1. Adopt and publish the [Acceptable AI Use Policy](acceptable-use-policy.md) template, customized for your organization;
2. Identify and formally approve at least one enterprise-grade AI tool with a signed DPA;
3. Run a mandatory 30-minute awareness session for all employees on AI data risks.

### 🟡 Moderate (65–84): 90-Day Programme
1. Complete the [Vendor Audit Checklist](vendor-audit-checklist.md) for all currently approved AI tools;
2. Conduct a DPIA for any AI workflow that processes Confidential or Restricted data;
3. Implement the [Deployment Decision Matrix](deployment-decision-matrix.md) as a mandatory gate for all new AI initiatives.

### 🟢 Managed (85–100): Continuous Improvement
1. Review and update all AI policies every 6 months, or immediately following significant regulatory changes (e.g., the 2 August 2026 EU AI Act deadline);
2. Establish a formal AI Governance Committee with representation from Legal, IT, and Business Operations;
3. Consider publishing your AI governance approach externally as a trust signal to clients and partners.

---

> **Context:** According to IBM's 2024 Cost of a Data Breach Report, the average cost of a data breach globally is **$4.88 million**. Breaches involving Shadow AI or unauthorized third-party tools add a significant premium to this figure. Gartner predicts that by 2027, 40% of enterprise AI-related security incidents will be attributable to Shadow AI. The cost of prevention is orders of magnitude lower than the cost of a breach.

---
*This calculator is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework. It is a self-assessment tool and does not constitute a formal security audit.*

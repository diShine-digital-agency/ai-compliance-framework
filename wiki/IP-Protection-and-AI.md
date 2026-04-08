# IP Protection and AI

The use of AI tools in enterprise environments creates specific intellectual property risks. When employees enter proprietary information into AI systems — particularly consumer-grade services — the organisation's trade secrets, copyrighted works, and confidential business information may be exposed.

## Core Risks

### 1. Trade Secret Loss

Under the **EU Trade Secrets Directive (2016/943)**, a trade secret retains its protected status only if the holder has taken **"reasonable steps"** to keep it secret (Article 2(1)(c)). If an employee pastes proprietary source code, business strategies, or customer data into a consumer AI tool, this may constitute a failure to take reasonable steps, potentially destroying trade secret protection.

The **Samsung ChatGPT incident (March 2023)** demonstrated this risk at scale: Samsung semiconductor engineers pasted proprietary source code and confidential meeting notes into ChatGPT, resulting in IP exposure. Samsung subsequently banned the use of generative AI tools.

### 2. Copyright Exposure

Two dimensions of copyright risk:

**Input side:** Feeding copyrighted material into an AI tool may constitute unauthorised reproduction. The EU text and data mining exception (Directive 2019/790, Article 4) permits reproduction for purposes of text and data mining, but rights holders can **opt out** of this exception. Providers of GPAI models must respect these opt-outs.

**Output side:** AI-generated content may reproduce elements of copyrighted works from the training data. The legal status of AI-generated output under EU copyright law is still evolving, but using output that substantially reproduces copyrighted material creates infringement risk.

### 3. Confidentiality Breach

Information shared with AI tools may be:
- **Stored** by the provider for service improvement, debugging, or moderation
- **Used for model training** (especially in consumer-tier services)
- **Accessible** to the provider's employees
- **Subject to legal process** (e.g., discovery in litigation)
- **Potentially leaked** through the model's responses to other users (memorisation risk)

## The Five Protection Techniques

The repository's [Prompt Engineering IP Protection Guidelines](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/prompt-ip-guidelines.md) define five techniques for preventing IP leakage:

### 1. Redaction and Anonymisation
Replace all identifying and proprietary information before submitting to an AI tool:
- Company names → "[Company A]"
- Product names → "[Product X]"
- Financial figures → "[$XX million]"
- Code-specific identifiers → generic placeholders

### 2. Abstraction and Generalisation
Describe problems at a level of abstraction that does not reveal proprietary details:
- Instead of "Our patented algorithm uses XYZ approach with parameters ABC," ask "What are best practices for optimising a classification algorithm?"
- Focus on the general pattern, not the specific implementation

### 3. Decomposition and Incremental Prompting
Break complex problems into smaller, independent sub-problems:
- Each sub-problem should be self-contained and not reveal the overall system architecture
- No single prompt should contain enough information to reconstruct the proprietary system

### 4. Structure-Focused (Not Content-Focused) Prompts
Ask for structural guidance rather than content:
- "What is a good structure for a patent application in the [domain] field?" rather than providing the actual invention details
- "Review this document structure" rather than "Review this confidential document"

### 5. Synthetic Data
When AI assistance requires data:
- Generate synthetic data that preserves statistical properties but contains no real information
- Use differential privacy techniques to create datasets that cannot be reverse-engineered to identify individuals or reveal proprietary information

## Deployment Tier Considerations

The [Deployment Decision Matrix](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/deployment-decision-matrix.md) maps data sensitivity to appropriate AI deployment tiers:

| Data Classification | Minimum Deployment Tier | Rationale |
|---|---|---|
| **Public** | Tier 1 (Consumer APIs) | No IP risk from public information |
| **Internal** | Tier 2 (Enterprise APIs with DPA) | Requires contractual protections against training use |
| **Confidential** | Tier 3 (Private Cloud / VPC) | Data must remain within organisational infrastructure |
| **Restricted** (trade secrets, regulated data) | Tier 4 (Self-Hosted Open-Source) | Zero external data exposure |

## Policy Integration

IP protection should be embedded in:

1. **Acceptable AI Use Policy** — explicitly define what data can and cannot be used with AI tools. The [Acceptable AI Use Policy template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/acceptable-use-policy.md) maps data classification to approved AI tiers.
2. **AI Literacy Programme** — include IP protection training for all employees. The [AI Literacy Programme template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-literacy-programme.md) includes this in the core curriculum.
3. **Vendor Contracts** — include IP protection clauses in AI vendor agreements (training data opt-out, output ownership, confidentiality obligations).
4. **Technical Controls** — DLP policies, URL filtering, endpoint monitoring to prevent sensitive data from reaching unauthorised AI services.

## GPAI Copyright Obligations

Under the EU AI Act, providers of GPAI models must:
- Put in place a **copyright compliance policy** (Article 53)
- Respect text and data mining **opt-outs** from rights holders
- Publish a sufficiently detailed **summary of training data content**

Organisations that fine-tune GPAI models on proprietary data should ensure their copyright policy complies with these requirements. See [General Purpose AI (GPAI)](General-Purpose-AI-GPAI).

---

**See also:** [Shadow AI: Risks and Mitigation](Shadow-AI) · [AI Vendor Due Diligence](AI-Vendor-Due-Diligence) · [General Purpose AI (GPAI)](General-Purpose-AI-GPAI) · [Algorithmic Bias and Fairness](Algorithmic-Bias-and-Fairness) · [Home](Home)

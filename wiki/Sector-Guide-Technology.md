# Sector Guide: Technology

Technology companies face unique obligations under the EU AI Act because they may simultaneously be **providers** (developers of AI systems), **deployers** (users of AI systems internally), and **distributors** (making AI available through platforms and marketplaces). The correct classification determines the applicable obligations.

## Provider vs. Deployer

| Scenario | Role | Obligations |
|---|---|---|
| You develop an AI-powered HR screening SaaS product | **Provider** of a high-risk AI system | Full high-risk compliance: conformity assessment, technical documentation, CE marking, EU AI Database registration, post-market monitoring |
| You use a third-party AI tool for your own recruitment | **Deployer** of a high-risk AI system | Human oversight, FRIA, log retention, transparency to candidates |
| You build a general-purpose chatbot platform | **Provider** of a limited-risk AI system + potentially **provider** of a GPAI model | Article 50 transparency; if providing a GPAI model, Articles 53–55 |
| You offer a cloud platform where customers deploy their own AI models | Potentially **distributor** or infrastructure provider | Due diligence, compliance verification |
| You fine-tune a GPAI model and deploy it as a product | **Provider** of the downstream AI system | Full obligations based on the risk classification of the resulting system |

## When Does a SaaS Product Become High-Risk?

The risk classification depends on the **intended purpose**, not the underlying technology:

| Product Category | Typical Risk Classification |
|---|---|
| AI-powered **recruitment** tools | High-risk (Annex III, Point 4) |
| AI-powered **credit scoring** | High-risk (Annex III, Point 5(b)) |
| AI-powered **EdTech** (grading, admissions) | High-risk (Annex III, Point 3) |
| AI-powered **biometric identification** | High-risk (Annex III, Point 1) |
| AI-powered **critical infrastructure** management | High-risk (Annex III, Point 2) |
| **Chatbots** and virtual assistants | Limited risk (Article 50 transparency) |
| **Content generation** tools (text, image, video) | Limited risk (deepfake labelling) |
| **Internal analytics** dashboards | Generally minimal risk |
| **Recommendation engines** (content, e-commerce) | Generally minimal risk |
| **Spam filters** | Minimal risk |

## NIS2 Obligations for Technology Companies

Technology companies that are **essential or important entities** under NIS2 (which includes providers of digital infrastructure, cloud computing services, data centre services, managed security services, and certain online platforms) face additional obligations:

- **Risk management** for network and information systems, including AI systems
- **Supply chain security** — cybersecurity requirements for suppliers and service providers
- **Incident reporting** — significant cybersecurity incidents must be reported within 24 hours (initial notification) and 72 hours (detailed report)
- **Business continuity** planning
- **Governance** — management body responsible for cybersecurity measures

## Cyber Resilience Act (CRA)

Technology companies placing products with digital elements on the EU market must comply with the CRA:

- **Security by design** — cybersecurity must be considered from the product design stage
- **Vulnerability handling** — procedures for receiving, analysing, and addressing vulnerability reports
- **Software updates** — security updates must be provided for the expected lifetime of the product
- **CE marking** — products must demonstrate compliance with CRA cybersecurity requirements
- **Documentation** — technical documentation including cybersecurity risk assessment

For AI-enabled products, both CRA and AI Act conformity assessment obligations may apply concurrently.

## Article 50 Transparency for Tech Products

Technology companies must ensure compliance with Article 50 transparency obligations:

| Product Type | Obligation |
|---|---|
| **Chatbots** | Inform users they are interacting with an AI system (unless obvious from context) |
| **Deepfake generators** | Generated/manipulated content must be machine-readably labelled as AI-generated |
| **Synthetic content tools** | Text published to inform the public must be labelled as AI-generated (unless editorially reviewed) |
| **Emotion recognition systems** | Inform exposed persons of the system's operation |

## Open-Source Considerations

The AI Act has a partial exemption for **free and open-source AI systems**:
- Open-source AI systems are generally exempt from provider obligations
- **Exception:** The exemption does **not** apply if the system is placed on the market as a high-risk system or if it falls within prohibited practices
- **GPAI models** released under open-source licences still have some obligations (training data summary, copyright compliance) unless released under a qualifying permissive licence with specific conditions

## Framework Templates

| Need | Template |
|---|---|
| Provider vs. Deployer role analysis | [Technology Sector Addendum](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-tech.md) |
| GPAI model obligations | [GPAI Model Governance Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/gpai-model-governance-checklist.md) |
| Deployment architecture decisions | [Deployment Decision Matrix](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/deployment-decision-matrix.md) |
| Conformity assessment pathway | [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md) |
| Cybersecurity alignment | [AI Incident Response Playbook](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/ai-incident-response-playbook.md) |

---

**See also:** [EU AI Act Roles](EU-AI-Act-Roles) · [General Purpose AI (GPAI)](General-Purpose-AI-GPAI) · [Open-Source AI and the EU AI Act](Open-Source-AI-and-the-EU-AI-Act) · [Transparency Obligations (Article 50)](Transparency-Obligations) · [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI) · [Conformity Assessment](Conformity-Assessment) · [Home](Home)

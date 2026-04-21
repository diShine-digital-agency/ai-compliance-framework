# EU AI Act Risk Classification

The EU AI Act uses a **risk-based approach** to regulate AI systems. The level of regulatory obligation is proportional to the potential harm an AI system may cause to health, safety, or fundamental rights. Systems are classified into four tiers.

## The Four Risk Tiers

### 1. Unacceptable Risk — Prohibited (Article 5)

AI practices that pose a clear threat to fundamental rights are **banned outright**. The prohibition has been in force since **2 February 2025**.

Prohibited practices include:

| Practice | Description |
|----------|-------------|
| **Social scoring** | AI systems that evaluate or classify natural persons based on social behaviour or personal characteristics, leading to detrimental treatment disproportionate or unrelated to the original context |
| **Subliminal manipulation** | Deploying techniques beyond a person's consciousness to materially distort their behaviour, causing or likely to cause significant harm |
| **Exploitation of vulnerabilities** | Targeting specific groups (age, disability, social or economic situation) in ways that materially distort their behaviour |
| **Real-time remote biometric identification in public spaces** | Use by law enforcement, except in narrowly defined exceptional cases (missing children, imminent terrorist threat, serious criminal offence investigation) |
| **Emotion recognition in workplaces and educational institutions** | AI systems that infer emotions of employees or students, with limited exceptions for medical or safety purposes |
| **Biometric categorisation based on sensitive characteristics** | Categorising individuals using biometric data to deduce race, political opinions, trade union membership, religious beliefs, sex life, or sexual orientation |
| **Untargeted facial image scraping** | Creating or expanding facial recognition databases through untargeted scraping from the internet or CCTV footage |
| **Predictive policing based solely on profiling** | Making risk assessments of natural persons to predict criminal offences based solely on profiling or personality traits |

**Penalty for violation:** Up to €35 million or 7% of global annual turnover.

For detailed guidance, see [Prohibited AI Practices](Prohibited-AI-Practices).

### 2. High Risk — Permitted with Strict Requirements (Articles 6–15, Annex III)

AI systems used in sensitive domains are classified as **high-risk** and are subject to comprehensive compliance requirements. These obligations come into force on **2 December 2027** under the Digital Omnibus proposal (**2 August 2026** remains legally binding until the Omnibus is adopted; legacy systems in regulated products receive additional time until 2 August 2028).

**Annex III high-risk use cases include:**

| Domain | Examples |
|--------|----------|
| **Biometric identification and categorisation** | Remote biometric identification (non-real-time), biometric categorisation |
| **Critical infrastructure** | Safety components of road traffic, water, gas, heating, electricity supply |
| **Education and vocational training** | AI for admissions, assessment of learning outcomes, exam proctoring |
| **Employment and workers management** | CV screening, interview analysis, performance evaluation, task allocation |
| **Access to essential services** | Credit scoring, insurance pricing, benefit eligibility assessment |
| **Law enforcement** | Polygraphs, evidence assessment, profiling in criminal investigations |
| **Migration, asylum, and border control** | Risk assessment, document verification |
| **Administration of justice and democracy** | AI assisting judicial authorities in legal research and case law interpretation |

**Requirements for high-risk systems:**

1. Risk management system (Article 9)
2. Data governance and management (Article 10)
3. Technical documentation (Article 11)
4. Record-keeping and logging (Article 12)
5. Transparency and information to deployers (Article 13)
6. Human oversight (Article 14)
7. Accuracy, robustness, and cybersecurity (Article 15)
8. Conformity assessment before market placement (Article 43)
9. EU AI Database registration (Article 49)
10. Post-market monitoring (Article 72)

**Additionally**, deployers of high-risk systems must conduct a **Fundamental Rights Impact Assessment** (Article 27) in certain cases.

AI systems that are **safety components of products** already covered by EU harmonisation legislation (medical devices, machinery, toys, lifts, radio equipment, in vitro diagnostics, civil aviation, motor vehicles, rail systems) are also high-risk and must go through the conformity assessment procedure of the relevant sectoral legislation.

For detailed guidance, see [High-Risk AI Systems](High-Risk-AI-Systems) and [Conformity Assessment](Conformity-Assessment).

**Framework template:** [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md), [Conformity Assessment Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/conformity-assessment-guide.md)

### 3. Limited Risk — Transparency Obligations (Article 50)

AI systems that interact with people or generate synthetic content have **transparency obligations** only.

| Obligation | Scope |
|------------|-------|
| **Chatbot disclosure** | Users must be informed they are interacting with an AI system (unless obvious from the circumstances) |
| **Deepfake labelling** | AI-generated or manipulated image, audio, or video content must be labelled as artificially generated or manipulated |
| **Emotion recognition/biometric categorisation disclosure** | Persons exposed to such systems must be informed of their operation |
| **AI-generated text disclosure** | Text published for the purpose of informing the public on matters of public interest must be labelled as AI-generated (unless subject to human editorial review) |

### 4. Minimal Risk — No Specific Obligations

The vast majority of AI systems fall into this category. Examples include spam filters, AI in video games, inventory management systems, and basic recommendation engines.

No specific AI Act obligations apply, though:
- General EU law (GDPR, product safety, consumer protection) still applies.
- Voluntary codes of conduct are encouraged.
- AI literacy obligations (Article 4) apply to providers and deployers regardless of risk level.

## How to Classify Your AI System

The classification process involves two steps:

**Step 1:** Determine whether the AI system falls within any of the **prohibited practices** listed in Article 5. If yes, the system cannot be deployed.

**Step 2:** If not prohibited, check whether the system:
- Is a **safety component** of a product covered by EU harmonisation legislation listed in Annex I, **or**
- Falls within a **use case** listed in Annex III

If either condition is met, the system is **high-risk** (unless the system does not pose a significant risk of harm — the so-called "filtering mechanism" in Article 6(3)).

**Step 3:** If not high-risk, check whether the system generates content, interacts with people, or performs emotion recognition or biometric categorisation. If yes, **limited risk** transparency obligations apply.

**Step 4:** If none of the above apply, the system is **minimal risk**.

The repository's [Deployment Decision Matrix](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/deployment-decision-matrix.md) and [Interactive Compliance Toolkit](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/tools/compliance-toolkit.html) (Deployment Tier Advisor) help organisations navigate this classification.

## Important Nuances

- **The same underlying model can be classified differently depending on the use case.** A large language model used for internal document summarisation is minimal risk; the same model used for CV screening is high-risk.
- **The classification obligation sits with the provider.** However, if a deployer uses a system in a way that changes its intended purpose, the deployer may become a provider and inherit the corresponding obligations.
- **Commission guidelines on high-risk classification** were required by February 2026 (Article 6(5)) to provide further clarity on borderline cases.

---

**See also:** [EU AI Act Overview](EU-AI-Act-Overview) · [High-Risk AI Systems](High-Risk-AI-Systems) · [Prohibited AI Practices](Prohibited-AI-Practices) · [Transparency Obligations (Article 50)](Transparency-Obligations) · [EU AI Act Roles](EU-AI-Act-Roles) · [Home](Home)

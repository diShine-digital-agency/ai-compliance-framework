# Frequently Asked Questions

## About the Framework

### What is this framework?
The AI Compliance Framework is an open-source collection of Markdown templates, guides, and an interactive toolkit for adopting AI responsibly in European corporate environments. It covers the EU AI Act, GDPR, and related regulations with practical, ready-to-use templates. See [About This Framework](About-This-Framework).

### Who is this framework for?
CEOs, CTOs, CISOs, DPOs, Legal Counsel, HR managers, Procurement officers, Data Scientists — anyone responsible for AI governance in an organisation operating in the EU. See the [role-based reference](About-This-Framework) for specific guidance by role.

### How do I start using the framework?
Start with the [Step-by-Step User Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/how-to-use-this-framework.md) in the repository. It maps the full compliance journey across four phases: Assess & Contain, Audit & Procure, Architect & Deploy, and Monitor & Respond.

### Can I use these templates in my organisation?
Yes. The framework is licensed under the MIT License. You are free to use, modify, and distribute the templates within your organisation. See the [LICENSE](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/LICENSE) file.

### Does using this framework make me legally compliant?
No. This framework provides informational guidance and templates to support your compliance efforts. It does not constitute legal advice. Compliance depends on your specific circumstances and requires assessment by qualified legal counsel.

### How do I contribute?
See the [Contributing Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/CONTRIBUTING.md). Contributions are welcome for regulatory corrections, new sector addenda, template improvements, and translations.

---

## EU AI Act — General

### What is the EU AI Act?
The EU AI Act (Regulation (EU) 2024/1689) is the world's first comprehensive legal framework for artificial intelligence. It entered into force on 1 August 2024 and establishes a risk-based regulatory framework. See [EU AI Act Overview](EU-AI-Act-Overview).

### When does the EU AI Act take effect?
The Act entered into force on 1 August 2024. Prohibited practices and AI literacy obligations have been in force since February 2025. GPAI obligations since August 2025. High-risk requirements and the full penalty regime take effect on 2 August 2026. See [EU AI Act Enforcement Timeline](EU-AI-Act-Enforcement-Timeline).

### Does the EU AI Act apply to my organisation?
If you develop, deploy, import, or distribute AI systems that affect persons in the EU, the Act likely applies to you — regardless of where your organisation is established. See [EU AI Act Overview](EU-AI-Act-Overview) for the full scope.

### What are the penalties for non-compliance?
Up to €35 million or 7% of global turnover for prohibited practices; €15 million or 3% for high-risk non-compliance; €7.5 million or 1% for incorrect information. See [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines).

---

## Risk Classification

### How do I know if my AI system is high-risk?
Check whether it is a safety component of a product covered by Annex I harmonisation legislation, or falls within a use case listed in Annex III (biometrics, critical infrastructure, education, employment, essential services, law enforcement, migration, justice). See [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification).

### Can the same AI model be classified differently for different uses?
Yes. The classification depends on the intended purpose, not the underlying technology. A large language model used for internal document summarisation is minimal risk; the same model used for CV screening is high-risk.

### What if my AI system is minimal risk?
No specific AI Act obligations apply, but GDPR, product safety, and consumer protection laws still apply. The AI literacy obligation (Article 4) applies to all providers and deployers regardless of risk level.

---

## GDPR and AI

### Do I need a DPIA for my AI system?
A DPIA is mandatory under GDPR Article 35 when processing is likely to result in a high risk to individuals. AI systems involving profiling, automated decision-making, large-scale processing of special category data, or systematic monitoring generally require a DPIA. See [DPIA for AI](DPIA-for-AI).

### What is the difference between a DPIA and an FRIA?
A DPIA (GDPR Article 35) focuses on personal data protection risks. An FRIA (AI Act Article 27) assesses broader fundamental rights impacts (dignity, non-discrimination, workers' rights, etc.). Both may be required for the same high-risk AI system. See [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment).

### Does GDPR Article 22 apply to AI decisions?
If your AI system makes or substantially informs decisions that produce legal or similarly significant effects on individuals (hiring, credit, insurance, benefits), Article 22 likely applies. Safeguards include the right to human intervention, the right to contest, and meaningful information about the logic involved.

---

## Practical Compliance

### What is Shadow AI and how do I address it?
Shadow AI is the use of AI tools by employees without organisational approval. It creates IP, GDPR, and AI Act risks. Mitigation involves an acceptable use policy, technical controls, approved alternatives, and AI literacy training. See [Shadow AI: Risks and Mitigation](Shadow-AI).

### How do I vet an AI vendor?
Use the 25-point [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) covering GDPR compliance, AI Act classification, and security/IP requirements. Key items include training data opt-out, data residency, risk classification, and bias testing. See [AI Vendor Due Diligence](AI-Vendor-Due-Diligence).

### Do I need ISO 42001 certification?
ISO 42001 certification is not legally required by the EU AI Act. However, it provides evidence of governance maturity, prepares the organisation for regulatory inspections, and may contribute to demonstrating compliance once harmonised European standards reference its principles. See [ISO 42001 and AI Governance Standards](ISO-42001-and-AI-Governance-Standards).

### What training do employees need?
Article 4 requires all providers and deployers to ensure staff dealing with AI systems have sufficient AI literacy. Training should be role-based: executives need governance awareness, technical staff need model governance skills, all employees need acceptable use and IP protection knowledge. See [AI Literacy Obligation](AI-Literacy-Obligation).

---

## Sector-Specific

### I work in financial services. What specific rules apply?
Credit scoring, insurance pricing, and loan approval AI are high-risk under Annex III. You also face DORA, MiFID II, and GDPR Article 22 obligations. See [Sector Guide: Financial Services](Sector-Guide-Financial-Services).

### I work in healthcare. When is our AI a medical device?
If your AI system has a medical purpose (diagnosis, treatment, prevention, monitoring), it likely qualifies as a medical device under the MDR and is automatically high-risk under the AI Act. See [Sector Guide: Healthcare](Sector-Guide-Healthcare).

### I work in HR. Can we use AI for recruitment?
Yes, but AI recruitment tools are high-risk under Annex III. You must ensure meaningful human oversight (not rubber-stamping), conduct bias testing, comply with Article 22, and consult Works Councils where required. Emotion recognition in interviews is prohibited. See [Sector Guide: Human Resources](Sector-Guide-Human-Resources).

### I work in education. What AI rules apply to schools and universities?
AI systems used for admissions, grading, and exam proctoring are high-risk under Annex III, Point 3. Emotion recognition in educational institutions is prohibited. Students have the right to explanation and human review of automated decisions. See [Sector Guide: Education](Sector-Guide-Education).

### I work in government. What extra obligations apply?
Public bodies deploying high-risk AI must conduct a Fundamental Rights Impact Assessment with public disclosure and register as deployers in the EU AI Database. Social scoring by public authorities is prohibited. See [Sector Guide: Public Administration and Government](Sector-Guide-Public-Administration).

---

## Transparency and Content Labelling

### Do I need to label AI-generated content?
Yes. Article 50 requires providers of AI systems that generate synthetic content (text, image, audio, video) to ensure outputs are marked in a machine-readable format as artificially generated. Deployers publishing deepfakes must additionally provide human-readable disclosure. See [Transparency Obligations (Article 50)](Transparency-Obligations).

### Does the AI Act apply to open-source AI models?
Partially. Open-source AI systems are generally exempt from provider obligations under Article 2(12), but the exemption does NOT apply if the system is high-risk, falls within prohibited practices, or triggers Article 50 transparency obligations. Open-source GPAI models with systemic risk are never exempt. See [Open-Source AI and the EU AI Act](Open-Source-AI-and-the-EU-AI-Act).

### What are regulatory sandboxes and how can I participate?
AI regulatory sandboxes are supervised testing environments established by national authorities under Article 57 where AI systems can be developed and tested under regulatory guidance. Every Member State must have at least one by August 2026. Participants benefit from regulatory certainty and protection from administrative fines during sandbox engagement. See [AI Regulatory Sandboxes](Regulatory-Sandboxes).

### What should my board be doing about AI governance?
The board should approve an AI governance policy, establish an AI governance committee, maintain an AI risk register, and receive structured AI governance reporting. AI compliance is a board-level responsibility — fines can reach 7% of global turnover. See [AI Governance and Board Oversight](AI-Governance-and-Board-Oversight).

### What are harmonised standards and when will they be ready?
Harmonised standards are European standards developed by CEN/CENELEC that create a presumption of conformity with AI Act requirements. Most are still in development (spring 2026) and are not expected to be fully available until late 2026 or 2027. Organisations should not wait for them — use ISO 42001 and Commission guidance in the interim. See [Harmonised Standards](Harmonised-Standards).

---

**See also:** [Home](Home) · [Glossary](Glossary) · [Key Regulatory References and Resources](Key-Regulatory-References)

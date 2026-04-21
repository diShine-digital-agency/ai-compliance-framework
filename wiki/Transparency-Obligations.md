# Transparency Obligations (Article 50)

Article 50 of the EU AI Act establishes transparency obligations for providers and deployers of certain AI systems. These obligations define the **limited risk** tier of the AI Act's risk-based framework and apply to AI systems that interact with people, generate synthetic content, or perform emotion recognition or biometric categorisation.

Article 50 obligations will be **fully enforceable from 2 November 2026** under the Digital Omnibus proposal (**2 August 2026** pre-Omnibus).

## Who Must Comply

| Obligation | Duty Bearer |
|---|---|
| Disclosure of AI interaction | **Provider** of the AI system |
| Machine-readable labelling of AI-generated content | **Provider** of the AI system |
| Deepfake disclosure | **Deployer** publishing AI-generated/manipulated content |
| Emotion recognition / biometric categorisation notification | **Deployer** of the system |
| Synthetic text disclosure (public interest) | **Deployer** publishing AI-generated text |

## The Four Transparency Duties

### 1. AI Interaction Disclosure (Article 50(1))

**Requirement:** Providers must design AI systems that interact directly with natural persons so that those persons are informed they are interacting with an AI system — unless this is **obvious from the circumstances and context of use**.

**Applies to:**
- Chatbots and virtual assistants
- AI customer service agents
- AI-driven phone systems
- Interactive AI tutoring systems

**Exceptions:**
- When it is obvious to a reasonably well-informed, observant, and circumspect person that they are interacting with an AI (e.g., a clearly labelled chatbot widget)
- AI systems authorised by law for the detection, prevention, investigation, or prosecution of criminal offences (subject to appropriate safeguards)

**Practical implementation:**
- Display a clear notice (e.g., "You are chatting with an AI assistant") at the start of the interaction
- Ensure the notice is visible and not buried in terms of service
- For voice-based systems, provide an audible disclosure before or at the start of the interaction

### 2. AI-Generated Content Labelling (Article 50(2))

**Requirement:** Providers of AI systems that generate synthetic audio, image, video, or text content must ensure that the outputs are marked in a **machine-readable format** as artificially generated or manipulated.

**Applies to:**
- Generative AI tools (text, image, audio, video)
- Large language models producing text
- AI image generators (DALL-E, Midjourney, Stable Diffusion equivalents)
- AI voice synthesis tools
- AI video generation/manipulation tools

**Technical implementation options:**
- **Watermarking** — embedding imperceptible signals in generated content that can be detected by automated tools
- **Metadata tagging** — encoding provenance information in file metadata (e.g., EXIF, XMP, C2PA)
- **Cryptographic signatures** — using digital signatures to certify content provenance and authenticity
- **Content Credentials (C2PA)** — the Coalition for Content Provenance and Authenticity standard for media authentication

**Requirements for marking:**
- Must be machine-readable (not just human-readable)
- Must be effective and robust (resistant to trivial removal)
- Must be interoperable (work across platforms and tools)
- Must be adapted to the content type
- Must be accessible via public tools or APIs for verification

**Exceptions:**
- AI systems performing assistive functions for standard editing (e.g., grammar correction, spell checking) where the AI does not substantially alter the content
- Systems authorised by law for criminal investigation purposes

### 3. Deepfake Disclosure (Article 50(4))

**Requirement:** Deployers who publish AI-generated or AI-manipulated image, audio, or video content that constitutes a **deepfake** must disclose that the content has been artificially generated or manipulated.

**Definition:** A deepfake is AI-generated or manipulated content (image, audio, video) that resembles existing persons, objects, places, or events and would **falsely appear to a person to be authentic or truthful**.

**Applies to:**
- Manipulated video/audio of real people
- AI-generated realistic imagery of persons
- Voice cloning and synthetic speech presenting as a real person
- Marketing content featuring AI-generated or manipulated visuals of real people

**The disclosure must be:**
- Clear and visible
- Placed at the point of publication/distribution
- Not hidden in metadata alone — human-readable disclosure is required for deployers

**Exceptions:**
- Content that is part of a manifestly artistic, creative, satirical, or fictional work, where the AI-generated nature is clear from the context
- Content authorised by law for criminal investigation purposes

### 4. Emotion Recognition and Biometric Categorisation Disclosure (Article 50(3))

**Requirement:** Deployers of AI systems that perform **emotion recognition** or **biometric categorisation** must inform the natural persons exposed to the system of its operation and process personal data in accordance with GDPR.

**Important:** This obligation concerns disclosure for *lawful* uses of emotion recognition and biometric categorisation. Certain uses of these technologies are entirely **prohibited** under Article 5 — see [Prohibited AI Practices](Prohibited-AI-Practices):
- Emotion recognition in the workplace (except for medical/safety purposes) — **prohibited**
- Emotion recognition in educational institutions — **prohibited**
- Biometric categorisation by sensitive attributes (race, religion, sexual orientation, etc.) — **prohibited**

## AI-Generated Text for Public Interest (Article 50(4))

Where AI-generated text is published with the purpose of **informing the public on matters of public interest**, deployers must disclose that the text was artificially generated — unless:
- The AI-generated content has undergone a process of **human review or editorial control**
- A natural person or legal entity holds **editorial responsibility** for the publication

This is particularly relevant for:
- AI-generated news articles
- Automated financial or sports reports
- AI-generated summaries of public documents
- AI-produced educational or informational content

## The EU Code of Practice on Transparency

The European Commission, through the EU AI Office, is developing a **Code of Practice on AI Labelling and Transparency** (also referred to as the Transparency Code of Practice). Key features:

- Provides detailed technical guidance for implementing Article 50 obligations
- Covers labelling methods, detection tools, and verification mechanisms
- Expected to serve as the de facto compliance benchmark, even though formally voluntary
- Draft published in January 2026; final version expected mid-2026
- Adherence to the Code of Practice may serve as evidence of compliance

## Interaction with Other Obligations

| Other Obligation | Interaction with Article 50 |
|---|---|
| **GDPR transparency (Arts. 13–14)** | Article 50 disclosure is additional to, not a substitute for, GDPR privacy notices. Both must be fulfilled. |
| **GDPR Article 22 (automated decisions)** | If the AI system makes or informs decisions with legal/significant effects, Article 22 requires meaningful information about the logic involved — beyond the simple disclosure required by Article 50. |
| **EU AI Act Article 13 (high-risk transparency)** | High-risk systems have more extensive transparency obligations under Article 13, in addition to any Article 50 obligations. Article 50 is the minimum for limited-risk systems. |
| **Digital Services Act** | VLOPs must also comply with DSA recommender system transparency and algorithmic content moderation obligations. |
| **Consumer protection law** | Unfair commercial practices rules may impose additional disclosure requirements for AI-powered marketing. |

## Penalties for Non-Compliance

Failure to comply with Article 50 transparency obligations can result in fines of up to **€15 million or 3% of global annual turnover**, whichever is higher (Article 99(4)(b)).

## Practical Compliance Checklist

1. **Inventory** all AI systems that interact with natural persons, generate content, or perform emotion recognition/biometric categorisation.
2. **Classify** each system against the four Article 50 duties.
3. **Implement AI interaction disclosure** — add visible notices to chatbots, virtual assistants, and interactive AI systems.
4. **Implement content labelling** — adopt machine-readable marking (watermarking, metadata, C2PA) for all AI-generated content.
5. **Implement deepfake disclosure** — add human-readable labels to any AI-generated or manipulated media that could be mistaken for real.
6. **Implement emotion recognition/biometric categorisation notices** — inform exposed persons and ensure GDPR compliance.
7. **Monitor the Transparency Code of Practice** — align implementation with the Commission's technical guidance as it is finalised.
8. **Document compliance** — maintain records of disclosure mechanisms, technical implementations, and any exceptions applied.

## Framework Templates

| Need | Template |
|---|---|
| AI use policy with transparency rules | [Acceptable AI Use Policy](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/acceptable-use-policy.md) |
| Content labelling for GPAI outputs | [GPAI Model Governance Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/gpai-model-governance-checklist.md) |
| Technology sector transparency | [Technology Sector Addendum](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-tech.md) |
| Vendor audit (transparency verification) | [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) |

---

**See also:** [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification) · [Prohibited AI Practices](Prohibited-AI-Practices) · [General Purpose AI (GPAI)](General-Purpose-AI-GPAI) · [GDPR and AI](GDPR-and-AI) · [Sector Guide: Technology](Sector-Guide-Technology) · [Home](Home)

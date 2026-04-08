# Open-Source AI and the EU AI Act

The EU AI Act contains a **partial exemption** for free and open-source AI systems under Article 2(12). Understanding the scope and limits of this exemption is critical for organisations that develop, contribute to, or deploy open-source AI models.

## The Open-Source Exemption (Article 2(12))

Article 2(12) provides that the AI Act **does not apply** to AI systems released under free and open-source licences.

**However, this exemption does not apply if:**

1. The AI system is placed on the market or put into service as a **high-risk AI system** (Annex I or Annex III)
2. The AI system falls within the **prohibited AI practices** of Article 5
3. The AI system is subject to the **transparency obligations** of Article 50

In other words, the open-source label does **not** provide blanket immunity. The exemption is narrowly scoped.

## What Remains Exempt

| Scenario | Exempt? |
|---|---|
| Open-source AI tool used internally for document summarisation (minimal risk) | ✅ **Yes** — minimal risk, open-source exemption applies |
| Open-source AI model shared on GitHub/HuggingFace for general use (minimal risk) | ✅ **Yes** — minimal risk, open-source exemption applies |
| Open-source chatbot library (limited risk — Article 50) | ❌ **No** — Article 50 transparency obligations still apply |
| Open-source recruitment screening tool (high-risk) | ❌ **No** — high-risk obligations apply in full |
| Open-source emotion recognition system used in the workplace | ❌ **No** — prohibited under Article 5 |
| Open-source credit scoring model | ❌ **No** — high-risk under Annex III |
| Open-source medical diagnostic AI | ❌ **No** — high-risk under Annex I (MDR) |

## Open-Source GPAI Models (Articles 53–55)

General-Purpose AI models released under open-source licences receive a **reduced set of obligations**, but are not fully exempt.

### Standard GPAI Models (Article 53)

GPAI providers normally must comply with four baseline obligations:
1. Technical documentation (Annex XI)
2. Information to downstream providers (Annex XII)
3. Copyright compliance policy
4. Training data summary publication

**Open-source reduction:** For GPAI models released under a qualifying open-source licence, obligations 1 and 2 are reduced. The provider must still:
- **Publish a sufficiently detailed summary of the training data** used to train the model
- **Comply with copyright requirements** — respect text and data mining opt-outs from rights holders

### GPAI Models with Systemic Risk (Article 55)

GPAI models that exceed the **10²⁵ FLOP** training compute threshold (or are designated by the Commission as posing systemic risk) are subject to additional obligations:
- Model evaluation and adversarial red-teaming
- Systemic risk assessment and mitigation
- AI Office incident reporting
- Cybersecurity protections

**The open-source exemption does NOT apply to GPAI models with systemic risk.** Even if a systemic-risk model is released under a fully open-source licence, the full set of Article 55 obligations applies.

## What Qualifies as "Open Source"?

The AI Act does not adopt a single strict definition of "open source." However, recitals and Commission guidance indicate that qualifying open-source AI must:

- Be made available under a licence that allows **free access, use, modification, and redistribution**
- Make the model's **parameters** (weights) publicly available
- Make the model's **architecture** and usage information public
- Not impose conditions that effectively restrict commercial use in ways inconsistent with open-source principles

**Note:** "Open weights" alone may not qualify if the licence restricts commercial use. Licences such as Meta's Llama licence (which restricts use above certain thresholds) may not meet the open-source exemption criteria.

## Practical Implications

### For Organisations Using Open-Source AI

1. **Do not assume exemption** — the open-source status of a model does not automatically exempt your use from the AI Act.
2. **Classify by use case** — the risk classification depends on what you use the model for, not whether the model is open-source. Using Llama for CV screening creates a high-risk system regardless of the model's open-source status.
3. **Article 50 still applies** — if you deploy an open-source chatbot, you must still comply with AI interaction disclosure obligations.
4. **GDPR still applies** — the open-source exemption only covers AI Act obligations. GDPR, product safety, and other regulations are unaffected.
5. **Conduct vendor due diligence** — even for open-source models, assess training data provenance, bias, and copyright compliance. The [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md) applies.

### For Organisations Developing/Releasing Open-Source AI

1. **Training data obligations persist** — even with the open-source reduction, you must publish a training data summary and comply with copyright opt-outs.
2. **Systemic risk models are never exempt** — if your model exceeds the 10²⁵ FLOP threshold, all GPAI obligations apply regardless of licence.
3. **Monitor downstream use** — if your open-source model is being used in high-risk applications, the deployer (not you as the open-source provider) bears the high-risk obligations, but you may still face liability under the Product Liability Directive if the model is defective.
4. **Document openly** — making technical documentation and safety information freely available may be both a good practice and a compliance asset.

### For Fine-Tuning Open-Source Models

If your organisation fine-tunes an open-source GPAI model and deploys it as a product:

- **You become the provider** of the downstream AI system (Article 25 — role transfer for substantial modification)
- The risk classification of the resulting system depends on its intended purpose
- You bear the full obligations of a provider for the downstream system
- The original open-source model provider's reduced obligations do not transfer to you

## Key Takeaway

The open-source exemption is best understood as follows:

> Open-source AI that is **minimal risk** and **does not interact with people** is largely exempt from AI Act obligations.
>
> Open-source AI that is **high-risk**, **prohibited**, or **triggers transparency obligations** receives no exemption — it must comply with the same rules as proprietary AI.
>
> Open-source **GPAI models** get reduced (but not eliminated) obligations, unless they pose **systemic risk**, in which case full obligations apply.

## Authoritative Resources

- [EU AI Act Article 2 — Scope](https://artificialintelligenceact.eu/article/2/)
- [Orrick — The EU AI Act: Application to Open-Source Projects](https://www.orrick.com/en/Insights/2024/09/The-EU-AI-Act-Application-to-Open-Source-Projects)
- [Linux Foundation — What Open Source Developers Need to Know about the EU AI Act](https://linuxfoundation.eu/newsroom/ai-act-explainer)

---

**See also:** [EU AI Act Overview](EU-AI-Act-Overview) · [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification) · [General Purpose AI (GPAI)](General-Purpose-AI-GPAI) · [Transparency Obligations (Article 50)](Transparency-Obligations) · [Sector Guide: Technology](Sector-Guide-Technology) · [Home](Home)

# Sector Guide: Beauty and Cosmetics

The beauty and cosmetics industry is increasingly adopting AI for virtual try-on, skin analysis, personalised product recommendations, AI-generated influencer content, and safety assessment. Several of these applications intersect with EU AI Act obligations around biometric categorisation, transparency, and health data.

## AI Use Cases and Risk Classification

| Use Case | AI Act Classification | Key Concern |
|---|---|---|
| **Virtual try-on** (AR makeup, hair colour) | Limited risk (Article 50 transparency if generating deepfake-like content) | Deepfake labelling if manipulated images are shared |
| **Skin analysis / diagnostics** | Potentially high-risk if crossing into medical device territory | MDR applicability; GDPR Article 9 if health data |
| **Personalised product recommendations** | Generally minimal risk | Standard GDPR obligations |
| **AI influencers / virtual brand ambassadors** | Limited risk (Article 50 transparency) | Must be disclosed as AI-generated content |
| **Shade matching / colour analysis** | Generally minimal risk, but biometric categorisation concerns | Article 5(1)(g) prohibition on biometric categorisation by sensitive attributes |
| **Sentiment analysis on reviews** | Minimal risk (unless inferring emotions of employees) | Prohibited if used for employee emotion recognition |
| **Safety assessment** | Depends on context — potentially high-risk if affecting product safety decisions | EU Cosmetics Regulation 1223/2009 interaction |

## Biometric Categorisation Prohibition

Article 5(1)(g) prohibits AI systems that categorise individuals using biometric data to deduce or infer sensitive attributes (race, religion, sexual orientation, etc.).

**Implications for beauty AI:**
- Skin tone analysis tools must be carefully designed to avoid categorising individuals by racial or ethnic origin
- Shade-matching AI should focus on colour properties (hue, saturation, value) rather than ethnic or racial categorisation
- Any system that uses facial analysis to infer sensitive characteristics is prohibited

## When Does Beauty AI Become a Medical Device?

The boundary between cosmetic and medical is critical:

| Claim | Classification |
|---|---|
| "This app helps you find the right foundation shade" | **Cosmetic** — minimal risk |
| "This app analyses your skin type for product recommendations" | **Cosmetic** — limited risk |
| "This app detects signs of melanoma in moles" | **Medical device** — high-risk under MDR |
| "This app diagnoses skin conditions and recommends treatment" | **Medical device** — high-risk under MDR |
| "This app monitors your skin health over time and alerts you to changes" | **Potentially medical** — depends on intended purpose and claims |

If an AI system crosses from cosmetic to diagnostic, it falls under the Medical Devices Regulation (MDR 2017/745) and is **automatically high-risk** under the AI Act. See [Sector Guide: Healthcare](Sector-Guide-Healthcare).

## GDPR Article 9 — When Is Skin Data Health Data?

Skin analysis that provides information about a person's health condition may constitute **health data** under GDPR Article 9:
- Identifying a skin condition = health data (special category)
- Identifying a skin tone for cosmetic matching = generally not health data (but biometric categorisation rules apply)

The distinction depends on the purpose and the nature of the information derived.

## AI-Generated Influencer Content

AI-generated virtual influencers and deepfake marketing content are subject to **Article 50 transparency obligations**:

- AI-generated images or videos of persons that are reasonably realistic must be labelled as AI-generated or manipulated
- Virtual brand ambassadors must be disclosed as non-human
- Marketing content created using AI must comply with consumer protection law and advertising standards

## EU Cosmetics Regulation (1223/2009)

The EU Cosmetics Regulation governs the safety of cosmetic products. If AI is used in the **safety assessment** process (required for all cosmetic products before market placement):
- The safety assessor retains responsibility for the assessment
- AI is a tool supporting, not replacing, the qualified safety assessor
- Documentation must demonstrate how AI was used and how the safety assessor validated the AI's output

## Framework Template

The repository's [Beauty & Cosmetics Sector Addendum](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-beauty.md) covers:
- Risk classification for beauty AI use cases
- Biometric categorisation prohibition analysis
- GDPR Article 9 health data boundary
- MDR crossover guidance
- Article 50 transparency for AI influencers
- Safety assessment considerations

---

**See also:** [EU AI Act Risk Classification](EU-AI-Act-Risk-Classification) · [Prohibited AI Practices](Prohibited-AI-Practices) · [GDPR and AI](GDPR-and-AI) · [Sector Guide: Healthcare](Sector-Guide-Healthcare) · [Home](Home)

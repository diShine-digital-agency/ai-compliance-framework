# AI Compliance Framework: Beauty & Cosmetics Addendum

**Version:** 1.0
**Regulatory Context:** April 2026

This addendum extends the core AI Compliance Framework for organizations operating in the Beauty and Cosmetics sector. It maps the core templates to sector-specific regulations including the EU Cosmetics Regulation (EC 1223/2009), the Medical Device Regulation (MDR), and GDPR special category data rules.

---

## 1. EU AI Act Risk Classification for Beauty

The beauty industry relies heavily on computer vision and generative AI. While many use cases are low risk, the boundary between cosmetic advice and medical diagnosis is easily crossed.

| AI Use Case | EU AI Act Classification | Key Regulatory Drivers |
| :--- | :--- | :--- |
| **Virtual Try-On (AR Filters)** | 🟢 **Limited Risk** | Must comply with Article 50 transparency (users must know it's AI). *Crucial: Do not use the biometric data to identify the user or infer sensitive traits.* |
| **Skin Analysis (Cosmetic)** | 🟢 **Limited Risk** | Recommending a moisturizer for "dry skin" is cosmetic. |
| **Skin Analysis (Diagnostic)** | 🔴 **High-Risk** (Annex III) | If the app diagnoses a condition (e.g., "rosacea" or "melanoma risk"), it becomes a Medical Device under MDR, and automatically a High-Risk AI system. |
| **AI Influencers / Deepfakes** | 🟢 **Limited Risk** | Article 50(3) and (4) require explicit, visible disclosure that the content (image/video) is artificially generated or manipulated. |

---

## 2. The Biometric Categorization Trap

The EU AI Act strictly regulates "biometric categorization."

*   **Acceptable:** Analyzing a face to map a lipstick shade to the lips.
*   **Prohibited (Article 5):** Using facial analysis to categorize a user by "racial or ethnic origin" to recommend products, *unless* you have explicit GDPR Article 9 consent.
*   **Action Item:** Ensure your `acceptable-use-policy.md` explicitly forbids the use of AI to infer race, ethnicity, or health status from user photos without explicit, documented legal review.

---

## 3. GDPR Article 9: When Skin Becomes "Health Data"

Under GDPR, "health data" is a special category requiring explicit consent (Article 9(2)(a)).

*   **The Boundary:** If your AI skin analysis tool identifies acne, eczema, or sun damage in a way that implies a medical condition requiring treatment, you are processing health data.
*   **The Fix:** If your tool is purely cosmetic, your UI copy must reflect this. Change "Diagnose your acne" to "Analyze your skin texture." If you *intend* to process health data, you must implement a robust consent flow and conduct a DPIA.

---

## 4. AI in Formulation and Safety Assessment

The EU Cosmetics Regulation (EC 1223/2009) requires a Cosmetic Product Safety Report (CPSR) signed by a qualified human safety assessor.

*   **AI as an Assistant:** AI can be used to predict toxicology or analyze ingredient interactions (in silico testing).
*   **The Human in the Loop:** AI *cannot* sign the CPSR. The human safety assessor must validate the AI's outputs. The AI's methodology and limitations must be documented in the Product Information File (PIF).

---

## 5. Immediate Action Plan (April 2026)

1.  **Audit Marketing Content:** Review all campaigns using virtual influencers or AI-generated models. Ensure clear, prominent disclosures are in place to comply with AI Act Article 50.
2.  **Review Skin Analysis Copy:** Audit the UX copy of any skin analysis tools. Remove any medical or diagnostic terminology to avoid accidentally triggering MDR and High-Risk AI Act classifications.
3.  **Check Biometric Data Flows:** Verify that photos uploaded for virtual try-on are processed ephemerally and not stored or used to train models without explicit consent.

---
*This addendum is provided by [diShine Digital Agency](https://dishine.it) as part of the AI Compliance Framework.*

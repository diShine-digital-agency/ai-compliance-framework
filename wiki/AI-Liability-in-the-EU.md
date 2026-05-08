# AI Liability in the EU

The EU has established a **two-pillar liability framework** for AI systems, after the AI Liability Directive proposal was withdrawn by the European Commission in 2025. Together, these instruments ensure that persons harmed by AI systems have effective legal remedies, while creating strong incentives for compliance with the EU AI Act.

## The Two Pillars

### Pillar 1: EU AI Act (Regulation (EU) 2024/1689) — The Rules

The AI Act establishes the compliance obligations that providers and deployers must meet. It defines what is required, sets penalties for non-compliance, and creates the foundation for liability claims.

Non-compliance with the AI Act has direct implications for liability: failing to meet AI Act requirements (e.g., risk management, human oversight, data governance) can be used as evidence of defectiveness in product liability claims and as evidence of breach of duty of care under national tort law.

### Pillar 2: Revised Product Liability Directive (2024/2853) — Strict Liability

| | |
|---|---|
| **Adopted** | November 2024 |
| **Transposition deadline** | 9 December 2026 |
| **Replaces** | Directive 85/374/EEC |
| **Liability type** | Strict (no-fault) |

The revised PLD makes several changes critical for AI:

**Software and AI are explicitly covered as "products."** Under the previous 1985 directive, software's status as a "product" was ambiguous. The revised directive removes this ambiguity.

**AI system outputs can constitute defects.** A product is defective if it does not provide the safety that a person is entitled to expect. For AI systems, this includes the safety implications of the system's outputs and decisions.

**Burden of proof lightening for claimants.** Where a claimant faces excessive difficulty in proving defectiveness or causation due to the technical or scientific complexity of the product (which is inherent in many AI systems), national courts may presume:
- That the product is defective, if the claimant demonstrates it is plausible
- That there is a causal link between the defect and the damage

**Non-compliance with mandatory requirements (including the AI Act) as evidence.** If a product does not comply with mandatory safety requirements, this constitutes evidence of defectiveness.

**Post-deployment learning liability.** The revised PLD covers defects arising from software updates, machine learning adaptations, or the lack of necessary updates. This means that an AI system that becomes harmful due to model drift or failure to update is still covered.

**Who is liable:**
- The **manufacturer** (provider in AI Act terms)
- The **importer** (if the manufacturer is outside the EU)
- The **authorised representative** (if applicable)
- The **distributor** (in certain circumstances)
- The **online platform** facilitating sales (if no EU-based manufacturer/importer is identified)

## Pillar 3 (Withdrawn): AI Liability Directive Proposal (COM/2022/496)

| | |
|---|---|
| **Proposed** | September 2022 |
| **Status** | **Withdrawn** by the European Commission |
| **Notice of withdrawal** | Published in the Official Journal on **6 October 2025** |
| **Commission decision** | 16 July 2025 (formalising the February 2025 work-programme intention) |

**Why it was withdrawn.** The Commission cited "no foreseeable agreement" among co-legislators after more than two years of stalled negotiations. The withdrawal was also driven by the regulatory simplification agenda underlying the Digital Omnibus package, and by the assessment that the revised Product Liability Directive plus AI Act compliance evidence already address most of the original AILD's purpose.

**What this means in practice.** There is currently **no fault-based AI-specific liability instrument at EU level**. Fault-based civil claims involving AI continue to be governed by **national tort law** in each Member State. Claimants who would have benefited from the AILD's harmonised presumption of causality and disclosure of evidence rules now rely on whatever equivalent mechanisms exist under their national civil procedure rules (which vary significantly).

**Possible future revival.** The Commission has signalled it may revisit the topic but has no active proposal as of May 2026. Practitioners should monitor the Commission's annual work programme.

## How the Two Pillars Interact

```
                ┌─────────────────┐
                │   Harm from AI  │
                └────────┬────────┘
                         │
            ┌────────────┴────────────┐
            │                         │
    ┌───────▼────────┐       ┌────────▼────────┐
    │ Product defect │       │ Fault / breach  │
    │ (no fault      │       │ of duty of care │
    │  required)     │       │                 │
    └───────┬────────┘       └────────┬────────┘
            │                         │
    ┌───────▼────────┐       ┌────────▼────────┐
    │ Revised PLD    │       │ National tort   │
    │ (strict        │       │ law of the      │
    │  liability)    │       │ Member State    │
    │                │       │ (AILD withdrawn)│
    └───────┬────────┘       └────────┬────────┘
            │                         │
            └────────────┬────────────┘
                         │
              ┌──────────▼──────────┐
              │ AI Act compliance   │
              │ status is evidence  │
              │ in both pathways    │
              └─────────────────────┘
```

In practice:
- **Strict liability (PLD):** The claimant must prove the product was defective and the defect caused the damage. Fault is irrelevant. Non-compliance with the AI Act is evidence of defectiveness.
- **Fault-based liability (national tort law):** The claimant must prove the defendant was at fault under the rules of their Member State. Non-compliance with the AI Act is generally treated by national courts as evidence of breach of duty of care, but the exact standard, the burden of proof and the disclosure mechanisms vary by jurisdiction.

Both pathways are available. Claimants choose the more favourable route under the law of the relevant Member State.

## Practical Implications

### For Providers
1. **Compliance with the AI Act is the primary defence** against both strict liability and national fault-based claims.
2. **Document everything.** Technical documentation, risk assessments, conformity assessment records, and post-market monitoring evidence are critical in defending liability claims.
3. **Post-deployment monitoring is essential.** The revised PLD covers defects arising after deployment (model drift, failure to update). Continuous monitoring and incident response are not optional.
4. **Track national tort developments.** With the AILD withdrawn, exposure now varies significantly across Member States. Map the rules of each market where you operate.

### For Deployers
1. **Deployers can face liability** under national tort law if they fail to meet their AI Act obligations (e.g., human oversight, incident reporting, FRIA). National courts generally treat AI Act non-compliance as evidence of breach of duty of care.
2. **Vendor due diligence is a protective measure.** Demonstrating that you vetted your AI vendor thoroughly (using the [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md)) strengthens your legal position.
3. **Contractual protections matter.** Ensure your contracts with AI providers include liability allocation, compliance representations, and indemnification clauses, with attention to which Member State's law applies and how that law treats AI-related claims.

### For All Organisations
1. **Insurance.** Consider AI-specific liability insurance, particularly for high-risk system deployments.
2. **Incident response preparedness.** A well-documented incident response capability (see [AI Incident Response](AI-Incident-Response)) demonstrates due diligence and can mitigate liability exposure.

## Framework Template

The repository's [AI Liability & Product Safety Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/ai-liability-product-safety.md) provides a comprehensive analysis of the two-pillar framework with practical guidance for providers and deployers, and tracks the implications of the AILD withdrawal.

---

**See also:** [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI) · [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines) · [AI Vendor Due Diligence](AI-Vendor-Due-Diligence) · [Conformity Assessment](Conformity-Assessment) · [Home](Home)

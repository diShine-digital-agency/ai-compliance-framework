# AI Liability in the EU

The EU has established a **three-pillar liability framework** for AI systems. Together, these three instruments ensure that persons harmed by AI systems have effective legal remedies, while creating strong incentives for compliance with the EU AI Act.

## The Three Pillars

### Pillar 1: EU AI Act (Regulation (EU) 2024/1689) — The Rules

The AI Act establishes the compliance obligations that providers and deployers must meet. It defines what is required, sets penalties for non-compliance, and creates the foundation for the two liability instruments.

Non-compliance with the AI Act has direct implications for liability: failing to meet AI Act requirements (e.g., risk management, human oversight, data governance) can be used as evidence of defectiveness or fault in liability claims.

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

### Pillar 3: AI Liability Directive (Proposed — COM/2022/496) — Fault-Based Liability

| | |
|---|---|
| **Proposed** | September 2022 |
| **Status** | Legislative process ongoing |
| **Liability type** | Fault-based, with presumption of causality |

The AILD addresses the specific challenges of bringing fault-based civil claims involving AI systems:

**Presumption of causality.** If a defendant (provider or deployer) has failed to comply with a **duty of care** (e.g., an AI Act obligation), and the resulting damage is the kind that the non-compliance was intended to prevent, the causal link between the fault and the damage is **presumed**. The defendant can rebut this presumption.

**Disclosure of evidence.** National courts can order providers or deployers to disclose relevant evidence about the AI system (training data, model architecture, decision logic). This addresses the "black box" problem where claimants cannot access the information needed to prove their case.

**Scope:** The AILD applies to both providers and deployers. Non-compliance with the AI Act (e.g., failure to implement adequate human oversight, inadequate risk management, insufficient data governance) provides the "fault" element.

## How the Three Pillars Interact

```
                ┌─────────────────┐
                │   Harm from AI  │
                └────────┬────────┘
                         │
            ┌────────────┴────────────┐
            │                         │
    ┌───────▼───────┐       ┌────────▼────────┐
    │ Product defect │       │ Fault / breach  │
    │ (no fault      │       │ of duty of care │
    │  required)     │       │                 │
    └───────┬───────┘       └────────┬────────┘
            │                         │
    ┌───────▼───────┐       ┌────────▼────────┐
    │ Revised PLD    │       │ AI Liability     │
    │ (strict        │       │ Directive        │
    │  liability)    │       │ (fault-based     │
    │                │       │  with causality  │
    │                │       │  presumption)    │
    └───────┬───────┘       └────────┬────────┘
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
- **Fault-based liability (AILD):** The claimant must prove the defendant was at fault (breached a duty of care). Non-compliance with the AI Act establishes the fault. Causality is presumed.

Both pathways are available. Claimants can choose the more favourable route.

## Practical Implications

### For Providers
1. **Compliance with the AI Act is the primary defence** against both strict and fault-based liability claims.
2. **Document everything.** Technical documentation, risk assessments, conformity assessment records, and post-market monitoring evidence are critical in defending liability claims.
3. **Post-deployment monitoring is essential.** The revised PLD covers defects arising after deployment (model drift, failure to update). Continuous monitoring and incident response are not optional.

### For Deployers
1. **Deployers can also face liability** under the AILD if they fail to meet their AI Act obligations (e.g., human oversight, incident reporting, FRIA).
2. **Vendor due diligence is a protective measure.** Demonstrating that you vetted your AI vendor thoroughly (using the [Vendor Audit Checklist](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/vendor-audit-checklist.md)) strengthens your legal position.
3. **Contractual protections matter.** Ensure your contracts with AI providers include liability allocation, compliance representations, and indemnification clauses.

### For All Organisations
1. **Insurance.** Consider AI-specific liability insurance, particularly for high-risk system deployments.
2. **Incident response preparedness.** A well-documented incident response capability (see [AI Incident Response](AI-Incident-Response)) demonstrates due diligence and can mitigate liability exposure.

## Framework Template

The repository's [AI Liability & Product Safety Guide](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/ai-liability-product-safety.md) provides a comprehensive analysis of the three-pillar framework with practical guidance for providers and deployers.

---

**See also:** [EU Regulatory Landscape for AI](EU-Regulatory-Landscape-for-AI) · [EU AI Act Penalties and Fines](EU-AI-Act-Penalties-and-Fines) · [AI Vendor Due Diligence](AI-Vendor-Due-Diligence) · [Conformity Assessment](Conformity-Assessment) · [Home](Home)

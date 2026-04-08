# Algorithmic Bias and Fairness

Algorithmic bias is one of the central concerns of the EU AI Act. Article 10 requires that training, validation, and testing data for high-risk AI systems be subject to appropriate data governance practices, with specific attention to possible biases. Article 15 requires that high-risk systems achieve appropriate levels of accuracy and avoid discriminatory impacts.

## What Is Algorithmic Bias

Algorithmic bias occurs when an AI system produces systematically unfair outcomes for certain groups of people, typically defined by protected characteristics (gender, race, age, disability, religion, sexual orientation). Bias can enter an AI system at multiple stages:

| Stage | Source of Bias |
|---|---|
| **Problem formulation** | The choice of what to predict or optimise may encode historical inequities |
| **Data collection** | Training data may underrepresent certain groups or reflect historical discrimination |
| **Data labelling** | Human annotators may introduce subjective biases into training labels |
| **Feature engineering** | Proxy variables (postcode, name, school attended) may correlate with protected characteristics |
| **Model training** | The optimisation process may amplify patterns that disadvantage minority groups |
| **Deployment context** | A model that is fair in one context may be unfair in another |
| **Feedback loops** | Model outputs influence future data collection, reinforcing existing biases |

## Fairness Metrics

The repository's [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) covers four core statistical fairness criteria:

### 1. Demographic Parity (Statistical Parity)
**Definition:** The probability of a positive outcome is the same across all groups.

P(Ŷ = 1 | A = a) = P(Ŷ = 1 | A = b) for all groups a, b

**Intuition:** The selection rate should be equal across groups, regardless of qualification rates.

### 2. Equal Opportunity
**Definition:** The true positive rate is the same across all groups.

P(Ŷ = 1 | Y = 1, A = a) = P(Ŷ = 1 | Y = 1, A = b)

**Intuition:** Among those who *should* receive a positive outcome, the AI system should identify them at the same rate regardless of group membership.

### 3. Equalized Odds
**Definition:** Both the true positive rate and the false positive rate are the same across all groups.

P(Ŷ = 1 | Y = y, A = a) = P(Ŷ = 1 | Y = y, A = b) for y ∈ {0, 1}

**Intuition:** The system should make errors at the same rate for all groups, for both positive and negative cases.

### 4. Predictive Parity
**Definition:** The positive predictive value (precision) is the same across all groups.

P(Y = 1 | Ŷ = 1, A = a) = P(Y = 1 | Ŷ = 1, A = b)

**Intuition:** Among those predicted to receive a positive outcome, the proportion who actually merit it should be the same across groups.

## The Impossibility Theorems

A critical finding in fairness research is that **it is mathematically impossible to satisfy all fairness metrics simultaneously** when the base rates (the true prevalence of the outcome) differ between groups:

- **Chouldechova (2017)** proved that when base rates differ, it is impossible to simultaneously achieve equal false positive rates, equal false negative rates, and equal positive predictive values.
- **Kleinberg, Mullainathan, and Raghavan (2016)** proved that calibration (predictive parity) and balance (equal false positive and false negative rates) cannot be simultaneously achieved when base rates differ.

**Practical implication:** Organisations must make an explicit, documented choice about which fairness criterion to prioritise, based on the legal and ethical context of the deployment. This choice should be recorded as part of the DPIA and FRIA documentation.

## The Four-Phase Audit Methodology

The bias audit methodology in the repository follows a structured four-phase approach:

### Phase 1: Pre-Audit Scoping
- Legal mapping: identify applicable anti-discrimination law (EU Employment Equality Directives, EU Charter Article 21, national law)
- Define protected characteristics to assess
- Define the fairness criteria appropriate to the use case
- Establish acceptable thresholds (e.g., 80% rule / four-fifths rule for disparate impact)

### Phase 2: Data Bias Audit
- Representation analysis: assess whether training data adequately represents all groups
- Label bias analysis: check for systematic labelling differences across groups
- Proxy variable identification: identify features that correlate with protected characteristics
- Historical bias assessment: determine whether the target variable itself encodes historical discrimination

### Phase 3: Model Bias Audit
- Calculate fairness metrics across all protected groups
- Test for disparate impact using the four-fifths rule
- Conduct counterfactual analysis: would the outcome change if the protected characteristic were different?
- Evaluate model calibration across groups

### Phase 4: Intersectional Audit
- Assess fairness at the intersection of multiple protected characteristics (e.g., gender × race × age)
- Identify subgroups that may be disproportionately affected
- Document findings and residual bias

## Bias Mitigation Strategies

| Strategy | When Applied | Trade-Off |
|---|---|---|
| **Pre-processing** | Before training — resampling, reweighting, or transforming training data | May reduce overall model accuracy |
| **In-processing** | During training — adding fairness constraints to the optimisation objective | May reduce model fit |
| **Post-processing** | After prediction — adjusting decision thresholds per group | May create different treatment by group |

Each strategy involves an **accuracy-fairness trade-off** that must be documented and justified.

## EU Legal Framework for Non-Discrimination

| Legislation | Scope |
|---|---|
| **EU Charter of Fundamental Rights, Article 21** | General prohibition of discrimination |
| **EU Employment Equality Directive (2000/78/EC)** | Discrimination in employment based on religion, disability, age, sexual orientation |
| **EU Gender Equality Directive (2006/54/EC)** | Equal treatment of men and women in employment |
| **EU Racial Equality Directive (2000/43/EC)** | Discrimination based on racial or ethnic origin in employment, social protection, education, goods and services |
| **EU AI Act, Article 10** | Data governance requirements for high-risk systems, including bias examination |
| **GDPR, Article 22** | Safeguards for automated decision-making affecting individuals |

## Framework Templates

| Resource | Purpose |
|---|---|
| [Algorithmic Bias Audit Methodology](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/guides/algorithmic-bias-audit-methodology.md) | Full 4-phase methodology with mathematical definitions |
| [DPIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/dpia-ai-template.md) | Bias risk section in the AI-specific DPIA |
| [FRIA Template](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/fria-template.md) | Non-discrimination impact assessment (Article 21 of the Charter) |
| [Sector Addendum: HR](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-hr.md) | Bias requirements for recruitment and employment AI |
| [Sector Addendum: Finance](https://github.com/diShine-digital-agency/ai-compliance-framework/blob/main/templates/sector-addendum-finance.md) | Bias requirements for credit scoring and insurance pricing |

---

**See also:** [DPIA for AI](DPIA-for-AI) · [Fundamental Rights Impact Assessment](Fundamental-Rights-Impact-Assessment) · [High-Risk AI Systems](High-Risk-AI-Systems) · [Sector Guide: Human Resources](Sector-Guide-Human-Resources) · [Home](Home)

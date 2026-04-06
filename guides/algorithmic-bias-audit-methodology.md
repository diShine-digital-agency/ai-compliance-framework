# Algorithmic Bias Audit Methodology Guide

**Version:** 1.4.0

As of 2026, algorithmic bias auditing has moved from an academic exercise to a strict regulatory requirement. Under the **EU AI Act (Article 10)**, providers of high-risk AI systems must implement data governance practices that specifically examine and mitigate biases likely to lead to discrimination. Concurrently, US regulations like NYC Local Law 144 and Colorado SB 205 mandate independent bias audits for automated decision tools.

This guide provides a rigorous, step-by-step methodology for conducting an algorithmic fairness audit. It moves beyond the simplistic "80% rule" to cover statistical fairness metrics, the mathematical impossibility theorems that govern them, and the specific requirements of Article 10(5) regarding the use of sensitive data for bias correction.

---

## 1. The Mathematical Reality of Fairness Metrics

Before conducting an audit, it is critical to understand that "fairness" is not a single mathematical concept. There are over 20 distinct statistical definitions of fairness, and **they are mathematically incompatible with each other** when base rates differ between groups [1].

### Core Statistical Fairness Criteria

When auditing a binary classification model (e.g., approve/deny loan, hire/reject candidate), you must choose which metric to optimize for based on the specific legal and ethical context of the use case.

| Metric | Mathematical Definition | Plain English | Best Used When... |
| :--- | :--- | :--- | :--- |
| **Demographic Parity** (Statistical Parity) | $P(\hat{Y}=1 \| A=0) = P(\hat{Y}=1 \| A=1)$ | The selection rate is identical across all demographic groups, regardless of the underlying ground truth. | Historical bias is so severe that the ground truth labels cannot be trusted (e.g., historical hiring data). |
| **Equal Opportunity** | $P(\hat{Y}=1 \| Y=1, A=0) = P(\hat{Y}=1 \| Y=1, A=1)$ | The True Positive Rate (TPR) is identical across groups. Qualified individuals have an equal chance of being selected. | The cost of a false negative (missing out on an opportunity) is high for the individual (e.g., loan approval). |
| **Equalized Odds** | $TPR_{A=0} = TPR_{A=1}$ AND $FPR_{A=0} = FPR_{A=1}$ | Both the True Positive Rate and False Positive Rate are identical across groups. | The cost of both false positives and false negatives is high and must be balanced. |
| **Predictive Parity** (Calibration) | $P(Y=1 \| \hat{Y}=1, A=0) = P(Y=1 \| \hat{Y}=1, A=1)$ | If the model predicts a positive outcome, the likelihood of it actually being positive is the same across groups. | The decision-maker needs to trust the model's confidence score equally for all groups (e.g., medical diagnosis). |

### The Impossibility Theorems

The Chouldechova (2017) and Kleinberg et al. (2016) impossibility theorems prove that **if the base rates (prevalence of the positive outcome) differ between two groups, it is mathematically impossible to simultaneously satisfy Equalized Odds and Predictive Parity** [1]. 

**Audit Implication:** You cannot simply tell a data science team to "make the model fair." The compliance, legal, and product teams must explicitly document *which* fairness metric they are prioritizing and *why*, acknowledging the mathematical trade-offs involved.

---

## 2. The 4-Phase Audit Methodology

### Phase 1: Pre-Audit Scoping & Legal Mapping
*   **Define the Protected Attributes:** Identify the specific demographic variables relevant to the jurisdiction. Under the EU Charter of Fundamental Rights (Article 21), this includes sex, race, colour, ethnic or social origin, genetic features, language, religion or belief, political or any other opinion, membership of a national minority, property, birth, disability, age, or sexual orientation.
*   **Establish the Baseline Metric:** Select the primary fairness metric (e.g., Equal Opportunity) based on the use case.
*   **Invoke Article 10(5) if Necessary:** The EU AI Act Article 10(5) provides a specific legal basis to process special categories of personal data (sensitive data) *strictly* for the purpose of bias detection and correction, provided state-of-the-art privacy measures (like pseudonymization) are used and the data is deleted once the bias is corrected [2].

### Phase 2: Data Bias Audit (Representation & Measurement)
Bias often originates in the training data before a model is even trained.
*   **Representation Analysis:** Calculate the demographic distribution of the training data. If a minority group constitutes less than 5% of the dataset, the model will likely suffer from high variance and error rates for that group.
*   **Label Bias Detection:** Analyze the ground truth labels. Are the historical decisions used to train the model already biased? (e.g., using past promotion data in a company with a history of gender disparity).
*   **Proxy Variable Identification:** Remove direct protected attributes (e.g., race), but also identify and evaluate highly correlated proxy variables (e.g., ZIP code, education institution) that can reconstruct the protected attribute.

### Phase 3: Model Bias Audit (Performance Disparity)
Evaluate the trained model's performance across demographic slices.
*   **Disparate Impact Analysis (The 80% Rule):** Calculate the selection rate for the protected group divided by the selection rate for the privileged group. While the US EEOC uses a 4/5ths (80%) threshold as a rule of thumb, EU audits should aim for statistical parity unless justified by objective, non-discriminatory factors [3].
*   **Error Rate Disparity:** Calculate the False Positive Rate (FPR) and False Negative Rate (FNR) for each group. A model that denies loans to qualified minority applicants (high FNR) at twice the rate of qualified majority applicants fails the Equal Opportunity test.
*   **Threshold Optimization:** Evaluate how changing the decision threshold (e.g., moving the approval cutoff from 0.5 to 0.6) impacts the fairness metrics across different groups.

### Phase 4: Intersectional Audit
Single-axis analysis (e.g., auditing for gender bias, then separately for racial bias) is insufficient. As demonstrated by intersectionality theory, bias often compounds at the intersection of identities (e.g., women of color may experience higher error rates than white women or men of color).
*   **Subgroup Slicing:** Segment the test data into intersectional groups (e.g., Gender x Race x Age).
*   **Statistical Power Check:** Ensure each intersectional subgroup has a sufficient sample size to achieve statistical significance. If data sparsity is an issue, document this limitation clearly in the audit report.

---

## 3. Bias Mitigation Strategies

If the audit reveals unacceptable disparities, the data science team must implement mitigation strategies. The audit report must document which strategy was chosen and its impact on overall model accuracy (the accuracy-fairness trade-off).

1.  **Pre-processing (Data Level):** Reweighting the training data to give more importance to underrepresented groups, or using techniques like SMOTE to oversample minority classes.
2.  **In-processing (Algorithm Level):** Adding a fairness constraint or regularization term to the model's loss function during training (e.g., adversarial debiasing), forcing the model to optimize for both accuracy and fairness simultaneously.
3.  **Post-processing (Decision Level):** Adjusting the decision thresholds differently for different groups to achieve the desired fairness metric (e.g., Equalized Odds post-processing). *Note: This approach carries high legal risk in some jurisdictions as it constitutes explicit disparate treatment to correct disparate impact.*

---

## 4. Documentation and EU AI Act Compliance

To comply with the EU AI Act's conformity assessment requirements for high-risk systems, the audit results must be formalized.

*   **Technical Documentation (Annex IV):** The audit methodology, the chosen fairness metrics, the results of the intersectional analysis, and the mitigation steps taken must be included in the system's technical documentation.
*   **Continuous Monitoring (Article 61):** Bias is not static. The post-market monitoring plan must include triggers for re-auditing the system if concept drift occurs or if the demographic composition of the user base changes significantly.

---

## References

[1] Chouldechova, A. (2017). Fair prediction with disparate impact: A study of bias in recidivism prediction instruments. *Big data*, 5(2), 153-163.
[2] European Parliament and Council. (2024). *Regulation (EU) 2024/1689 laying down harmonised rules on artificial intelligence (Artificial Intelligence Act)*. Article 10: Data and Data Governance.
[3] Feldman, M., Friedler, S. A., Moeller, J., Scheidegger, C., & Venkatasubramanian, S. (2015). Certifying and removing disparate impact. In *Proceedings of the 21th ACM SIGKDD international conference on knowledge discovery and data mining* (pp. 259-268).

*This guide is part of the AI Compliance Framework by diShine Digital Agency.*

---

> **Framework Navigation:** This document is part of the [AI Compliance Framework](../README.md) by [diShine Digital Agency](https://dishine.it). It is used in **Phase 3 — Architect & Deploy**, **Step 3.3: Audit for Algorithmic Bias**. For the full deployment sequence, rationale, and ownership guide, see the [Step-by-Step User Guide](how-to-use-this-framework.md).

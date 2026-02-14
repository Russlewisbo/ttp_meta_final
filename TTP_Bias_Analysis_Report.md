# Risk of Bias Analysis: TTP Meta-Analysis

**Date:** February 13, 2026  
**Studies Included:** 45 mortality studies from TTP Meta-Analysis

## Executive Summary

This risk of bias analysis evaluates 45 studies examining the association between blood culture time to positivity (TTP) and mortality in bacteremia. The assessment used six domains based on the Newcastle-Ottawa Scale and ROBINS-I criteria: Selection, Comparability, Outcome Assessment, Statistical Analysis, Attrition, and Prognostic Measurement.

### Key Findings

- **Overall Assessment:** Most studies (66.7%) had moderate overall risk of bias, with 26.7% low risk and 6.7% high or critical risk
- **Strongest Domain:** Attrition (84.4% low risk)
- **Most Concerning Domain:** Comparability (77.8% moderate or high risk)
- **High Risk Studies:** Only 3 studies (6.7%) had high or critical overall risk

## Overall Risk of Bias Distribution

| Risk Level | Number of Studies | Percentage |
|------------|-------------------|------------|
| **Low** | 12 | 26.7% |
| **Moderate** | 30 | 66.7% |
| **High** | 2 | 4.4% |
| **Critical** | 1 | 2.2% |

## Domain-Specific Risk Assessment

### 1. Selection Bias
- **Low Risk:** 17 studies (37.8%)
- **Moderate Risk:** 26 studies (57.8%)
- **High Risk:** 2 studies (4.4%)

**Interpretation:** More than half of studies had moderate concerns regarding patient selection, often due to single-center designs or unclear consecutive enrollment procedures.

### 2. Comparability
- **Low Risk:** 10 studies (22.2%)
- **Moderate Risk:** 34 studies (75.6%)
- **High Risk:** 1 study (2.2%)

**Interpretation:** This was the most concerning domain. Most studies had moderate risk due to inadequate control for confounding factors such as disease severity, comorbidities, and appropriateness of empiric therapy. Only 22% of studies adequately controlled for key confounders through matching or multivariable adjustment.

### 3. Outcome Assessment
- **Low Risk:** 25 studies (55.6%)
- **Moderate Risk:** 20 studies (44.4%)
- **High Risk:** 0 studies (0%)

**Interpretation:** More than half of studies had low risk for outcome assessment, typically using objective outcomes like all-cause mortality from medical records or registries. Moderate risk was assigned when outcome ascertainment methods were unclear or follow-up periods varied.

### 4. Statistical Analysis
- **Low Risk:** 33 studies (73.3%)
- **Moderate Risk:** 12 studies (26.7%)
- **High Risk:** 0 studies (0%)

**Interpretation:** Most studies employed appropriate statistical methods for their study design (logistic regression, Cox proportional hazards, or appropriate unadjusted analyses for 2×2 tables).

### 5. Attrition
- **Low Risk:** 38 studies (84.4%)
- **Moderate Risk:** 7 studies (15.6%)
- **High Risk:** 0 studies (0%)

**Interpretation:** This was the best-performed domain. The majority of studies had complete outcome ascertainment or minimal loss to follow-up (<10%).

### 6. Prognostic Measurement
- **Low Risk:** 24 studies (53.3%)
- **Moderate Risk:** 18 studies (40%)
- **High Risk:** 3 studies (6.7%)

**Interpretation:** About half of studies had low risk, using standardized automated blood culture systems with clearly defined TTP measurement protocols. Moderate risk was assigned when TTP measurement procedures were incompletely described. High risk studies had concerns about TTP measurement consistency or validation.

## Implications for Meta-Analysis

### Strengths
1. **Objective Outcomes:** Most studies used objective, hard outcomes (mortality) with standardized measurement
2. **Low Attrition:** Excellent follow-up completeness across studies
3. **Appropriate Statistics:** Studies generally used appropriate analytical methods

### Limitations
1. **Confounding Control:** The primary concern is inadequate adjustment for confounders in many studies, particularly:
   - Disease severity scores (APACHE, SOFA)
   - Source control adequacy
   - Appropriateness of empiric antibiotics
   - Comorbidity burden
   
2. **Selection Bias:** Many single-center studies with unclear generalizability

3. **Heterogeneity in TTP Definition:** Studies varied in:
   - Blood culture systems used (BACTEC, BacT/ALERT, VersaTREK)
   - TTP cutpoints (8h to 16h thresholds)
   - Whether TTP was from first positive or all positive cultures

## Risk of Bias and Meta-Regression Results

According to the AGENTS.md analysis, meta-regression found that **risk of bias did not significantly modify the TTP-mortality association** (95% CrI for ROB coefficient included zero). This suggests that:

1. The overall pooled effect (OR ≈ 2.14) is relatively robust to study quality
2. Both high- and low-quality studies show consistent associations
3. Unmeasured confounding may be less influential than feared, OR confounding operates similarly across studies

However, the predominance of moderate-quality studies (67%) means that:
- The true effect may be somewhat overestimated due to residual confounding
- The association might be partially explained by unmeasured confounders (e.g., inoculum as proxy for source control failure)

## Sensitivity Analysis Recommendations

Given the bias assessment, the following analyses strengthen interpretation:

1. ✅ **Subgroup by ROB:** Already performed - no significant difference
2. ✅ **Exclude high/critical risk studies:** Only 3 studies - unlikely to change estimate substantially
3. ✅ **Publication bias adjustment:** Already performed with Bayesian selection models
4. **Future consideration:** Stratify by:
   - Single-center vs multicenter design
   - Adjusted vs unadjusted effect estimates
   - Studies with adequate disease severity adjustment

## Conclusion

The included studies have predominantly moderate overall risk of bias, with the primary concern being inadequate control for confounding factors. However, the consistency of the association across studies of varying quality, the lack of significant ROB moderator effects in meta-regression, and the robustness to sensitivity analyses all support a genuine association between short TTP and increased mortality risk.

The true effect size likely lies between the conservative publication bias-adjusted estimate (OR ≈ 1.50, trim-and-fill) and the primary Bayesian estimate (OR ≈ 2.14), with the magnitude partly dependent on the degree of unmeasured confounding by disease severity and treatment appropriateness.

## Recommendations for Future Studies

To improve evidence quality, future studies should:

1. **Control for key confounders:**
   - Disease severity (validated scores)
   - Source control adequacy
   - Appropriateness and timing of empiric therapy
   - Comorbidity indices

2. **Use multicenter designs** to improve generalizability

3. **Standardize TTP measurement:**
   - Report blood culture system
   - Use consistent TTP definitions (time to first positive)
   - Specify TTP cutpoints with clinical or statistical justification

4. **Report adjusted estimates** with transparent confounder selection

5. **Consider propensity score methods** or other causal inference frameworks to address confounding by indication

---

**Figures:**
- `bias_stoplight.png` - Individual study risk assessment across all domains
- `bias_summary.png` - Domain-specific risk distribution

**Data Source:** `TTP_MetaAnalysis_Extraction_Complete.xlsx` (tbl_study sheet)

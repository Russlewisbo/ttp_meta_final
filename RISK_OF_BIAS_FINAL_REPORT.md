# Risk of Bias Assessment - Final Report
## TTP Meta-Analysis: Corrected Study Count

**Date:** February 19, 2026  
**Analysis:** Time to Positivity and Clinical Outcomes in Bacteremia

---

## Executive Summary

### Inclusion Criteria Met
- **54 studies** were potentially eligible after initial screening
- **36 unique studies** met all inclusion criteria and contributed analyzable effect sizes
- **42 total effect sizes** were included in the meta-analysis
  - 35 mortality effect sizes (33 unique studies)
  - 5 persistent bacteremia effect sizes
  - 2 microbiological clearance effect sizes

### Why 36 Studies, Not 40?

The original project documentation referenced "40 unique studies," but the accurate count is **36 studies**. The difference is due to:

1. **Studies with insufficient data** (n=14): Had PICO-compliant outcomes but lacked:
   - Complete 2×2 tables for effect size calculation, AND
   - Reported effect estimates with confidence intervals
   
2. **Studies with unusable effect estimates** (n=4): Reported outcomes in formats not convertible to odds ratios (e.g., continuous outcomes, severity scores)

### Multiple Effect Sizes

Six studies contributed **2 effect sizes each** (different outcomes or subgroups):
- **Cilloniz2017**: Adjusted and unadjusted mortality estimates
- **Hou2023**: Two different mortality outcomes
- **Marco2025**: Two genuinely different subgroups
- **Melling2019**: Mortality and persistent bacteremia
- **Minejima2019**: Mortality and persistent bacteremia
- **Ok2013**: Two different mortality outcomes

This accounts for 42 effect sizes from 36 studies (36 + 6 = 42).

---

## Overall Risk of Bias

### Distribution (n=36 studies)

| Risk Level | n | Percentage |
|-----------|---|-----------|
| **Low** | 10 | 27.8% |
| **Moderate** | 24 | 66.7% |
| **High** | 1 | 2.8% |
| **Critical** | 1 | 2.8% |

**Key Finding:** Two-thirds of studies (67%) had moderate risk of bias, primarily due to inadequate adjustment for confounders in the Comparability domain.

---

## Domain-Specific Risk of Bias

### Summary Table

| Domain | Low Risk | Moderate Risk | High Risk |
|--------|----------|--------------|-----------|
| **Selection** | 14 (38.9%) | 21 (58.3%) | 1 (2.8%) |
| **Comparability** | 10 (27.8%) | 25 (69.4%) | 1 (2.8%) |
| **Outcome Assessment** | 20 (55.6%) | 16 (44.4%) | 0 (0%) |
| **Statistical Analysis** | 27 (75.0%) | 9 (25.0%) | 0 (0%) |
| **Attrition** | 31 (86.1%) | 5 (13.9%) | 0 (0%) |
| **Prognostic Measurement** | 18 (50.0%) | 15 (41.7%) | 3 (8.3%) |

### Domain Analysis

#### 1. **Best Domain: Attrition (86.1% low risk)**
- Most studies had excellent follow-up completeness
- Minimal loss to follow-up for mortality outcomes
- Clear documentation of study flow

#### 2. **Most Problematic Domain: Comparability (69.4% moderate risk, 2.8% high risk)**
- **Main Issue:** Inadequate adjustment for confounders
- **Common unmeasured confounders:**
  - Disease severity scores (APACHE II, SOFA, Pitt bacteremia score)
  - Appropriateness of empiric antibiotic therapy
  - Source control adequacy and timing
  - Comorbidity burden (Charlson index)
  - Time to effective therapy

- **Why this matters:** TTP may be a proxy for disease severity. Without proper adjustment, the observed association could be confounded by baseline patient characteristics.

#### 3. **Selection Domain (38.9% low risk)**
- **Common issues:**
  - Convenience sampling from single centers
  - Retrospective designs with potential selection bias
  - Unclear inclusion/exclusion criteria

#### 4. **Prognostic Measurement (50.0% low risk, 8.3% high risk)**
- **Issues with TTP measurement:**
  - Variable blood culture systems (BacT/ALERT, BACTEC, etc.)
  - Different incubation protocols
  - Inconsistent cutpoint selection (data-driven vs. a priori)
  - Continuous vs. dichotomized analysis

- **High-risk studies:** Used data-driven cutpoints or had unclear TTP measurement protocols

#### 5. **Outcome Assessment (55.6% low risk)**
- Most studies used objective outcomes (mortality, persistent bacteremia)
- Some lacked blinding of outcome assessors
- Mortality is relatively robust to measurement bias

#### 6. **Statistical Analysis (75.0% low risk)**
- Most studies used appropriate statistical methods
- Good reporting of effect estimates and confidence intervals
- Some studies lacked multivariable adjustment

---

## Implications for Meta-Analysis Interpretation

### Strengths Despite Moderate Risk

1. **Robust outcomes:** Mortality is objective and hard to misclassify
2. **Consistent direction:** Despite heterogeneity, effect direction is consistent across studies
3. **No high attrition:** Follow-up completeness reduces bias from missing data
4. **Meta-regression tested ROB:** Overall risk of bias did NOT modify the TTP-mortality association (95% CrI for ROB coefficient included zero)

### Limitations to Consider

1. **Residual confounding:** The association may be partially explained by unmeasured severity
2. **Publication bias:** Significant funnel asymmetry suggests selective reporting
3. **Observational data:** All studies are observational (no RCTs)
4. **Heterogeneous TTP measurement:** Different cutpoints and systems complicate interpretation

### Clinical Validity

Despite moderate risk of bias, the findings appear **clinically valid** because:
- Effect size is consistent across different pathogen classes
- Association persists in adjusted analyses when reported
- Biological plausibility (higher inoculum → worse outcomes)
- Consistency with prior meta-analyses

---

## Studies with High/Critical Risk of Bias

### Critical Risk (n=1)
- **Hsieh 2022**: Meta-analysis with methodological concerns

### High Risk (n=1)
- **Ji 2020**: Multiple domains rated high risk
  - Poor prognostic measurement (unclear TTP definition)
  - Inadequate statistical analysis
  - High attrition

**Sensitivity Analysis:** Excluding Ji 2020 reduced the pooled OR from 2.14 to 2.00 (95% CrI: 1.61-2.47), indicating the main finding is robust even without this high-risk study.

---

## Recommendations for Future Research

### Study Design
1. **Prospective cohorts** with pre-specified TTP cutpoints
2. **Standardized TTP measurement** protocols across sites
3. **Comprehensive confounder adjustment:**
   - Disease severity scores
   - Appropriateness of empiric therapy
   - Time to source control
   - Comorbidity indices

### Reporting
1. Report both **continuous TTP** (per hour) and dichotomized analyses
2. Provide **adjusted and unadjusted** estimates
3. Document **blood culture system** and incubation protocol
4. Justify **TTP cutpoint selection** (a priori vs. data-driven)

### Dose-Response
Future meta-analyses should incorporate continuous TTP data to assess dose-response relationships and identify optimal cutpoints.

---

## Conclusion

The risk of bias assessment reveals that while most studies (67%) have **moderate overall risk**, the findings appear **robust and clinically valid**. The main concern is **residual confounding** due to inadequate adjustment for disease severity, but the consistency of findings across diverse populations and pathogen classes supports the validity of TTP as a prognostic marker in bacteremia.

**Take-Home Message:** The TTP-mortality association is likely real, though the magnitude may be partially explained by unmeasured confounders. TTP remains a valuable early warning sign that can be used immediately upon culture positivity to risk-stratify patients.

---

## Files Generated

1. **bias_stoplight_included.png** - Individual study risk assessment (10"×14")
2. **bias_summary_included.png** - Domain-specific risk distribution
3. **bias_overall_included.png** - Overall risk of bias distribution
4. **bias_complete_summary_included.png** - Combined publication-ready figure
5. **TTP_Bias_Assessment_Included_Details.csv** - Study-level assessment data
6. **TTP_Bias_Assessment_Included_Summary.csv** - Domain summary table
7. **TTP_Final_Included_Studies_ROB.csv** - Complete study list with ROB scores

---

**Assessment completed:** February 19, 2026  
**Assessor:** Russell Lewis  
**Tool:** QUIPS (Quality In Prognosis Studies)  
**Studies assessed:** 36 unique studies contributing 42 effect sizes

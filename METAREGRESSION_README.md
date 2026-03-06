# Meta-Regression Analysis: TTP-Mortality Association
## Exploring Sources of Heterogeneity

**Created:** February 19, 2026  
**Resolution:** 600 DPI (publication quality)  
**Style:** JAMA  
**Analyses:** 4 moderator variables tested

---

## Overview

This meta-regression analysis explores potential moderators that might explain the substantial heterogeneity (I² = 98.6%) observed in the TTP-mortality association. We tested four key moderators: pathogen class, risk of bias, publication year, and TTP cutpoint.

---

## Key Findings

### Main Result
**Only TTP cutpoint significantly moderated the association** (QM = 11.01, p < 0.001), explaining 27.3% of between-study heterogeneity and reducing residual I² from 98.6% to 71.3%.

### Moderator Test Results

| Moderator | Test Statistic (QM) | p-value | Significant? | I² Reduction |
|-----------|---------------------|---------|--------------|--------------|
| **TTP Cutpoint** | 11.01 | **<0.001** | ✅ **YES** | **27.3%** |
| Publication Year | 3.22 | 0.073 | ❌ No | 0.6% |
| Risk of Bias | 2.74 | 0.098 | ❌ No | 0.1% |
| Pathogen Class | 3.97 | 0.137 | ❌ No | 0.3% |

---

## Figure Files

### Figure 1: Forest Plot by Pathogen Class
**Filename:** `MetaReg_Figure1_Pathogen_Forest_JAMA.png`  
**Dimensions:** 10" × 12"  
**Resolution:** 600 DPI

**Description:**  
Stratified forest plot showing individual study effect sizes grouped by pathogen class (Gram-positive, Gram-negative, Mixed). Square size proportional to study precision.

**Finding:**  
No significant difference between pathogen subgroups (QM = 3.97, p = 0.137). Effect sizes similar across all three categories, confirming TTP as pathogen-agnostic marker.

---

### Figure 2: TTP Cutpoint Bubble Plot
**Filename:** `MetaReg_Figure2_TTP_Bubble_JAMA.png`  
**Dimensions:** 9" × 7"  
**Resolution:** 600 DPI

**Description:**  
Bubble plot showing relationship between TTP cutpoint (x-axis, in hours) and observed effect size (y-axis, odds ratio). Bubble size represents study precision (1/variance). Blue line shows linear regression fit with 95% CI.

**Finding:**  
**Significant negative association** (QM = 11.01, p < 0.001):
- Studies using shorter TTP cutpoints (e.g., 8-12 hours) report larger effect sizes (OR 4-8)
- Studies using longer cutpoints (e.g., 24+ hours) report smaller effect sizes (OR 1-2)
- **Interpretation:** This may reflect differential bacterial growth dynamics or selection of high-risk subgroups at shorter intervals

---

### Figure 3: Coefficient Plot for All Moderators
**Filename:** `MetaReg_Figure3_Coefficients_JAMA.png`  
**Dimensions:** 10" × 6"  
**Resolution:** 600 DPI

**Description:**  
Forest plot of meta-regression coefficients for all moderators. Shows point estimates (diamonds) with 95% confidence intervals. Significant moderators colored blue, non-significant gray.

**Coefficients (log-OR scale):**
- TTP Cutpoint (per hour): **-0.064** (95% CI: -0.102 to -0.026), p < 0.001 ✅
- Publication Year (per year): 0.042 (95% CI: -0.004 to 0.087), p = 0.073
- Risk of Bias (High vs Low/Moderate): -0.401 (95% CI: -0.883 to 0.081), p = 0.098
- Pathogen: Gram-Negative vs Gram-Positive: 0.342 (95% CI: -0.042 to 0.727), p = 0.068
- Pathogen: Mixed vs Gram-Positive: 0.516 (95% CI: -0.155 to 1.186), p = 0.126

---

### Figure 4: Residual Heterogeneity Reduction
**Filename:** `MetaReg_Figure4_Heterogeneity_JAMA.png`  
**Dimensions:** 10" × 6"  
**Resolution:** 600 DPI

**Description:**  
Horizontal bar chart showing residual I² after adding each moderator. Color intensity indicates degree of heterogeneity reduction (darker blue = more reduction).

**Finding:**  
- Baseline I² (no moderators): 98.6%
- After adding TTP cutpoint: 71.3% (27.3% reduction) ✅
- Other moderators: Minimal reduction (0.1-0.6%)

**Interpretation:**  
TTP cutpoint choice substantially explains heterogeneity, but 71.3% residual I² remains, suggesting other unmeasured factors (patient severity, antibiotic timing, source control) also contribute.

---

## Summary Table

### Table 4: Meta-Regression Results
**Filename:** `Table4_MetaRegression_Summary.html`  
**Format:** HTML (paste into Word)

**Content:**
- Studies included for each moderator (k)
- QM test statistic
- p-value
- Baseline and residual I²
- I² reduction (%)

**Highlighted:** TTP cutpoint row (pale blue background) showing significant result.

---

## Interpretation & Clinical Implications

### Why Does TTP Cutpoint Matter?

The significant moderator effect of TTP cutpoint has important implications:

**1. Biological Plausibility:**
- Shorter cutpoints (8-12h) capture patients with very high bacterial inocula
- Longer cutpoints (24h+) include wider range of bacterial loads
- Differential risk stratification at different thresholds

**2. Study Design Impact:**
- Choice of cutpoint is data-driven in many studies (optimal cutpoint from ROC analysis)
- This may amplify effect estimates in some studies
- Standardized cutpoints (e.g., 12h) needed for comparability

**3. Clinical Application:**
- Very short TTP (<12h) may be more specific for high-risk patients
- Moderate TTP (12-24h) still prognostic but weaker signal
- Longer TTP (24h+) may dilute prognostic value

### Why Don't Other Moderators Explain Heterogeneity?

**Pathogen Class (p = 0.137):**
- Consistent effect across Gram-positive, Gram-negative, and mixed infections
- Confirms TTP as universal prognostic marker
- Bacterial load matters more than organism type

**Risk of Bias (p = 0.098):**
- Trend toward larger effects in low-risk studies (better methodology)
- But not statistically significant
- Suggests findings robust to study quality

**Publication Year (p = 0.073):**
- Borderline trend toward larger effects in recent studies
- May reflect improved TTP measurement technology
- Or publication of higher-quality evidence over time

### Unmeasured Confounders

The high residual heterogeneity (71.3% after TTP cutpoint) likely reflects:

1. **Patient Severity:**
   - APACHE II / SOFA scores rarely reported
   - Comorbidity burden varies widely
   - ICU vs ward populations

2. **Treatment Factors:**
   - Appropriateness of empiric therapy
   - Time to effective antibiotics
   - Source control adequacy and timing

3. **Methodological:**
   - Adjusted vs unadjusted estimates
   - Different covariates in multivariable models
   - Confounding by indication

4. **Measurement:**
   - Different blood culture systems (BacT/ALERT, BACTEC)
   - Varying incubation protocols
   - Different TTP measurement precision

---

## Statistical Methods

### Models Fitted

All meta-regressions used restricted maximum likelihood (REML) with:

```r
rma(yi, vi, mods = ~ moderator, data = data, method = "REML")
```

### Test Statistics

**QM (Test of Moderators):**
- Omnibus test that all moderator coefficients = 0
- Chi-square distribution
- Significant QM indicates moderator explains heterogeneity

**Residual I²:**
- Heterogeneity remaining after accounting for moderator
- Lower residual I² = better explanatory power
- Calculated from residual Q statistic

### Interpretation of Coefficients

**Continuous Moderators (Year, TTP Cutpoint):**
- Coefficient = change in log-OR per unit increase in moderator
- TTP cutpoint: -0.064 log-OR per hour
  - Means: Each additional hour of TTP cutpoint associated with 6.2% reduction in OR

**Categorical Moderators (Pathogen, Risk of Bias):**
- Coefficient = difference in log-OR vs reference category
- Reference: Gram-Positive (pathogen), Low/Moderate (risk of bias)

---

## Recommendations for Future Research

### Standardize TTP Measurement
1. **Pre-specify cutpoints:** Use 12h as standard threshold (most common in literature)
2. **Report continuous TTP:** Include dose-response analyses
3. **Report multiple cutpoints:** Show sensitivity to threshold choice

### Measure Key Confounders
1. **Disease severity scores:** APACHE II, SOFA, Pitt bacteremia score
2. **Antibiotic timing:** Time to appropriate therapy
3. **Source control:** Achievability and timing
4. **Comorbidity:** Charlson index or similar

### Methodological Improvements
1. **Prospective designs:** Reduce selection bias
2. **Standardized blood culture systems:** Improve comparability
3. **Individual patient data meta-analysis:** Better control for confounding

---

## Limitations

### Analysis Limitations

1. **Ecological fallacy:** Study-level moderators may not reflect patient-level relationships
2. **Limited power:** Only 26-33 studies per moderator
3. **Measurement error:** Moderators extracted from study descriptions (may be imprecise)
4. **Multiple testing:** Four moderators tested (no adjustment for multiple comparisons)

### Data Limitations

1. **Missing data:** Not all studies reported all moderators
   - TTP cutpoint: Only 26/33 studies
   - Blood culture system: Only 32/33 studies

2. **Heterogeneous definitions:**
   - "High risk of bias" varies across domains
   - Pathogen class includes diverse organisms within each category
   - TTP cutpoint measurement may differ between systems

3. **Confounding:** Study-level covariates may be confounded with each other

---

## Files Generated

**Figures (4 total, 600 DPI):**
1. `MetaReg_Figure1_Pathogen_Forest_JAMA.png` (10"×12")
2. `MetaReg_Figure2_TTP_Bubble_JAMA.png` (9"×7")
3. `MetaReg_Figure3_Coefficients_JAMA.png` (10"×6")
4. `MetaReg_Figure4_Heterogeneity_JAMA.png` (10"×6")

**Tables:**
- `Table4_MetaRegression_Summary.html` - HTML table for Word
- `MetaRegression_Results.csv` - Raw data

**Documentation:**
- `METAREGRESSION_README.md` - This file

---

## Citation

When reporting these meta-regression analyses, cite:

> Lewis R. Time to Positivity in Bacteremia: Meta-Regression Analysis of Heterogeneity. [Journal]. 2026. [In preparation]

---

## Suggested Text for Manuscript

### Methods Section:

> "To explore sources of heterogeneity, we conducted univariable meta-regression analyses using restricted maximum likelihood (REML) estimation. We examined four potential moderators: pathogen class (Gram-positive, Gram-negative, mixed), overall risk of bias (low/moderate vs high/critical), publication year (continuous), and TTP cutpoint (continuous, in hours). The statistical significance of moderators was assessed using the QM test, and residual heterogeneity (I²) was calculated after accounting for each moderator."

### Results Section:

> "Meta-regression analyses revealed that TTP cutpoint significantly moderated the TTP-mortality association (QM = 11.01, p < 0.001), with shorter cutpoints associated with larger effect sizes (coefficient = -0.064 log-OR per hour, 95% CI -0.102 to -0.026). This explained 27.3% of between-study heterogeneity, reducing I² from 98.6% to 71.3%. Other moderators (pathogen class, risk of bias, publication year) did not significantly explain heterogeneity (all p > 0.05). The substantial residual heterogeneity suggests that unmeasured factors such as disease severity, antibiotic timing, and source control adequacy also contribute to between-study variability."

---

## Location

**Files saved in:** `/Users/russelllewis/Desktop/ttp_meta_final/`

---

**Last updated:** February 19, 2026

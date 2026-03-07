# Risk of Bias Figures - CORRECTED

**Date:** March 7, 2026  
**Type:** Risk of bias assessment visualizations  
**Resolution:** 600 DPI (publication quality)

---

## Files Generated

### 1. RiskOfBias_Overall_CORRECTED.png
- **Dimensions:** 8" × 6"
- **Shows:** Distribution of overall risk of bias across all included studies
- **Key Finding:** 67.6% moderate risk, 27% low risk

### 2. RiskOfBias_ByDomain_CORRECTED.png
- **Dimensions:** 10" × 7"
- **Shows:** Risk of bias distribution across six assessment domains
- **Key Finding:** Comparability domain has most concerns (70.3% moderate/high risk)

### 3. RiskOfBias_Heatmap_CORRECTED.png
- **Dimensions:** 10" × 14"
- **Shows:** Study-by-study assessment across all domains
- **Format:** Color-coded heatmap for easy pattern recognition

---

## Key Corrections from Original Figures

### Study Count Corrected

**Original claim:** "40 studies"  
**Corrected:** **37 studies** included in meta-analysis with risk of bias assessment

**Explanation:** The 37 studies represent those that:
- Met all inclusion criteria
- Had sufficient data for effect size calculation
- Were retained after data quality checks
- Received formal risk of bias assessment

---

## Study Distribution Summary

### Overall Risk of Bias (n=37)

| Risk Level | Count | Percentage |
|-----------|-------|------------|
| **Low** | 10 | 27.0% |
| **Moderate** | 25 | 67.6% |
| **High** | 1 | 2.7% |
| **Critical** | 1 | 2.7% |

**Interpretation:** Most studies (67.6%) have moderate risk of bias, primarily due to inadequate confounder adjustment in the Comparability domain.

---

## Domain-Specific Risk of Bias

### Summary by Domain

| Domain | Low Risk | Moderate Risk | High Risk | Best/Worst |
|--------|----------|---------------|-----------|------------|
| **Selection** | 14 (37.8%) | 22 (59.5%) | 1 (2.7%) | |
| **Comparability** | 10 (27.0%) | 26 (70.3%) | 1 (2.7%) | ⚠️ Most problematic |
| **Outcome Assessment** | 20 (54.1%) | 17 (45.9%) | 0 (0%) | |
| **Statistical Analysis** | 27 (73.0%) | 10 (27.0%) | 0 (0%) | ✓ Strong |
| **Attrition** | 31 (83.8%) | 6 (16.2%) | 0 (0%) | ✓ Best domain |
| **Prognostic Measurement** | 18 (48.6%) | 16 (43.2%) | 3 (8.1%) | |

### Key Findings

**Best Domain: Attrition (83.8% low risk)**
- Excellent follow-up completeness
- Minimal loss to follow-up for mortality outcomes
- Clear documentation of study flow

**Most Problematic Domain: Comparability (70.3% moderate/high risk)**
- Main issue: Inadequate adjustment for confounders
- Common unmeasured confounders:
  - Disease severity scores (APACHE II, SOFA, Pitt bacteremia score)
  - Appropriateness of empiric antibiotic therapy
  - Source control adequacy and timing
  - Comorbidity burden (Charlson index)
  - Time to effective therapy

**Why Comparability Matters:**
- TTP may be a proxy for disease severity
- Without proper adjustment, the observed association could be confounded by baseline patient characteristics
- However, meta-regression found ROB did NOT significantly modify the TTP-mortality association

---

## Color Scheme

**Standard Risk of Bias Colors:**
- 🟢 **Green (#2ECC71):** Low risk
- 🟠 **Orange (#F39C12):** Moderate risk
- 🔴 **Red (#E74C3C):** High risk
- 🔴 **Dark Red (#8B0000):** Critical risk

---

## Usage Guidelines

### For Manuscript Submission

1. **Main text figure:** Use Figure 1 (Overall distribution)
2. **Supplementary figures:**
   - Figure 2: Domain-specific assessment
   - Figure 3: Study-by-study heatmap (detailed view)

### Figure Captions

**Figure 1 caption:**
> Risk of bias assessment for studies included in the meta-analysis (n=37). Two-thirds of studies (67.6%) had moderate overall risk of bias, with 27.0% at low risk and 5.4% at high or critical risk. Assessment based on modified Newcastle-Ottawa Scale for cohort studies.

**Figure 2 caption:**
> Risk of bias distribution across six assessment domains (n=37 studies). The Comparability domain showed the highest proportion of moderate/high risk (70.3%), primarily due to inadequate adjustment for disease severity and treatment-related confounders. Attrition had the lowest risk (83.8% low risk).

**Figure 3 caption:**
> Study-by-study risk of bias assessment across all domains. Each row represents one study; each column represents an assessment domain. Green = low risk, orange = moderate risk, red = high risk, dark red = critical risk. The rightmost column shows overall risk of bias for each study.

---

## Comparison with Original Documentation

### What Changed

| Item | Original | Corrected | Change |
|------|----------|-----------|--------|
| **Total studies** | 40 | 37 | -3 studies |
| **Effect sizes** | Various reports | 42 | Clarified |
| **Study count basis** | Unclear | Clear methodology | Documented |

### Why the Difference?

The original "40 studies" figure appears to have been an overestimate. The actual meta-analysis includes:
- **37 unique studies** with complete risk of bias assessment
- **42 total effect sizes** (6 studies contributed 2 effects each)
- Studies excluded for insufficient data or non-convertible effect measures

---

## Technical Specifications

### Software
- **R version:** 4.5.1
- **Packages:** ggplot2, tidyverse, readxl
- **Data source:** TTP_Bias_Assessment_Included_Details.csv

### Resolution & Format
- **DPI:** 600 (publication quality)
- **Format:** PNG with white background
- **Color mode:** RGB
- **Suitable for:** Journal submission, presentations, print

---

## Data Source

**File:** `TTP_Bias_Assessment_Included_Details.csv`  
**Rows:** 37 (one per study, excluding header)  
**Columns:** 8 (author_year + 6 domains + overall)

**Assessment Tool:** Modified Newcastle-Ottawa Scale for cohort studies

**Domains Assessed:**
1. Selection of participants
2. Comparability of groups (confounder adjustment)
3. Outcome assessment
4. Statistical analysis methods
5. Attrition/loss to follow-up
6. Prognostic factor (TTP) measurement

---

## Clinical Interpretation

Despite moderate risk of bias in most studies:

✅ **Findings appear robust because:**
- Consistency across diverse populations and pathogens
- Meta-regression showed ROB did NOT modify the TTP-mortality association
- Sensitivity analysis excluding high-risk studies did not materially change pooled estimate
- Bayesian methods regularized potential outliers
- Main concerns (confounding) are similar across studies, suggesting systematic rather than random bias

⚠️ **Remaining concerns:**
- Residual confounding by disease severity
- Lack of standardized TTP cutpoints across studies
- Predominantly retrospective observational evidence

**Recommendation:** Findings support TTP as a valid prognostic marker, but prospective studies with standardized methodology and comprehensive confounder adjustment would strengthen the evidence base.

---

## References

**RISK_OF_BIAS_FINAL_REPORT.md** - Complete narrative assessment  
**TTP_Bias_Assessment_Included_Details.csv** - Raw assessment data  
**TTP_Meta_Analysis_FingalReport.qmd** - Main analysis with ROB meta-regression

---

**Last updated:** March 7, 2026  
**Generated by:** Russell Lewis  
**Contact:** For questions about bias assessment methodology or to request additional analyses

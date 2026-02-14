# TTP Meta-Analysis: Bias Analysis Outputs

## Overview

This folder contains a comprehensive risk of bias analysis for the 45 mortality studies included in the Time to Positivity (TTP) Meta-Analysis, as described in `TTP_Meta-Analysis_FingalReport.qmd` and based on the data in `AGENTS.md`.

**Analysis Date:** February 13, 2026  
**Analyst:** Russell Lewis  
**Studies Analyzed:** 45 mortality studies

## Files Generated

### Reports
1. **`TTP_Bias_Analysis_Report.md`** - Comprehensive narrative report including:
   - Executive summary
   - Overall risk of bias distribution
   - Domain-specific assessments
   - Implications for meta-analysis
   - Recommendations for future studies

### Data Files
2. **`TTP_Bias_Assessment_Details.csv`** - Complete study-level bias ratings with:
   - Study ID and publication year
   - Ratings for all 6 domains
   - Overall risk of bias classification

3. **`TTP_Bias_Assessment_Table.csv`** - Publication-ready formatted table

### Figures
4. **`bias_stoplight.png`** (10" × 14") - Individual study risk assessment
   - Rows: All 45 studies
   - Columns: 6 bias domains
   - Colors: Green (low), Yellow (moderate), Red (high)

5. **`bias_summary.png`** (10" × 6") - Domain-specific risk distribution
   - Stacked bar chart showing percentage breakdown
   - All 6 domains with risk level proportions

6. **`bias_complete_summary.png`** (12" × 10") - Combined comprehensive figure
   - Overall risk of bias distribution (bar chart)
   - Domain-specific risk distribution (stacked bars)
   - Publication-ready composite

## Key Results Summary

### Overall Risk of Bias
- **Low risk:** 12 studies (26.7%)
- **Moderate risk:** 30 studies (66.7%)  ⭐ Most common
- **High risk:** 2 studies (4.4%)
- **Critical risk:** 1 study (2.2%)

### Best Performing Domain
**Attrition** - 84.4% low risk
- Excellent follow-up completeness
- Minimal loss to follow-up

### Most Concerning Domain
**Comparability** - 77.8% moderate or high risk
- Inadequate control for confounding
- Key unmeasured confounders:
  - Disease severity (APACHE, SOFA scores)
  - Appropriateness of empiric therapy
  - Source control adequacy
  - Comorbidity burden

## Domain Breakdown

| Domain | Low Risk | Moderate Risk | High Risk |
|--------|----------|---------------|-----------|
| **Selection** | 37.8% | 57.8% | 4.4% |
| **Comparability** | 22.2% | 75.6% | 2.2% |
| **Outcome** | 55.6% | 44.4% | 0% |
| **Statistical Analysis** | 73.3% | 26.7% | 0% |
| **Attrition** | 84.4% | 15.6% | 0% |
| **Prognostic Measurement** | 53.3% | 40.0% | 6.7% |

## Implications for Primary Analysis

### Supporting Evidence for Robustness
1. **Meta-regression found no significant ROB moderator effect**
   - Association consistent across high and low quality studies
   - 95% CrI for ROB coefficient included zero

2. **Objective outcome (mortality) in most studies**
   - Hard endpoint with standardized measurement
   - Low risk of outcome assessment bias

3. **Only 3 studies (6.7%) at high/critical risk**
   - Excluding these unlikely to substantially change pooled estimate

### Remaining Concerns
1. **Residual confounding likely present**
   - 77.8% of studies had moderate/high comparability risk
   - True effect may be somewhat overestimated
   - Association might partly reflect unmeasured confounders

2. **Heterogeneity in TTP measurement**
   - Different blood culture systems
   - Variable cutpoints (8h to 16h)
   - Different measurement protocols

## Integration with Main Meta-Analysis

The bias analysis supports the conclusions in the main report:

1. ✅ **Association is robust** - Consistent across studies of varying quality
2. ✅ **Effect size uncertainty** - Publication bias and potential confounding suggest true effect between OR 1.50–2.14
3. ✅ **Sensitivity analyses appropriate** - ROB subgroup analysis, outlier exclusion, publication bias adjustments all strengthen interpretation

## Citation

When using these results, cite as:

> Lewis R. Risk of Bias Analysis: Time to Positivity Meta-Analysis. Supplementary Analysis. February 2026.

## Questions or Issues

For questions about the bias assessment methodology or interpretation, refer to:
- Main analysis: `TTP_Meta-Analysis_FingalReport.qmd`
- Study database: `TTP_MetaAnalysis_Extraction_Complete.xlsx` (tbl_study sheet)
- Project memory: `AGENTS.md`

---

**Generated:** February 13, 2026  
**Software:** R 4.5+ with tidyverse, ggplot2, readxl

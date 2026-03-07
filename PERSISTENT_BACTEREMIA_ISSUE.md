# Persistent Bacteremia Frequentist REML Issue

**Date:** March 7, 2026  
**Issue:** Frequentist REML produces clinically implausible results  
**Status:** Bayesian estimate should be preferred

---

## The Problem

The frequentist REML meta-analysis for persistent bacteremia produces an **implausible result**:

**Frequentist REML:**
- Pooled OR: **8.99**
- 95% CI: **1.67 – 48.29**
- I²: **99.2%**
- τ: **2.50**
- p-value: 0.0105

This result doesn't make clinical sense because:
1. **Extremely wide confidence interval** (1.67 to 48.29 = 29-fold range)
2. **Point estimate nearly 9× increased risk** seems implausibly high
3. **Dominated by extreme outliers** with sparse cell counts

---

## Root Cause: Extreme Outlier Studies

### Individual Study Effect Sizes

| Study | OR | 95% CI | Issue |
|-------|-----|--------|-------|
| **Melling2019** | **1722.25** | 236.97–12,517.22 | ⚠️ Extreme sparse cells |
| **Kassis2009** | **74.82** | 20.85–268.48 | ⚠️ Sparse cells |
| **Melling2019** | **37.45** | 20.60–68.11 | ⚠️ Sparse cells |
| **Ok2013** | **14.57** | 3.52–60.32 | ⚠️ Wide CI |
| **Choi2012** | **12.50** | 1.85–84.44 | ⚠️ Wide CI |
| Khatib2005 | 2.02 | 1.48–2.75 | ✓ Reasonable |
| Peri2026 | 1.59 | 1.06–2.39 | ✓ Reasonable |
| Minejima2019 | 1.17 | 1.06–1.29 | ✓ Reasonable |
| Ok2013 | 0.26 | 0.09–0.73 | Protective effect |

### The Outlier Problem

**Three effect sizes are driving the pooled estimate:**
1. **Melling2019** with OR = **1722** (!!!)
   - This is based on 2×2 table with very sparse cells
   - Adds 0.5 to zero cells, creating extreme estimate
   
2. **Kassis2009** with OR = **75**
   - 72/89 vs 3/56 events
   - Sparse cell in control group
   
3. **Melling2019** (second effect) with OR = **37**
   - Similar sparse cell issue

These three studies have enormous influence on the pooled estimate despite being methodologically questionable.

---

## Why Frequentist REML Fails Here

### 1. Small Sample Size
- Only **7 studies** (9 effect sizes)
- Insufficient for reliable random-effects estimation
- Tau estimate is very unstable (SE = 3.31)

### 2. Extreme Heterogeneity
- **I² = 99.2%** - nearly all variability is between-study
- Ranges from OR = 0.26 to OR = 1722
- No meaningful "average" effect exists

### 3. Sparse Cell Counts
- Several studies have zero or near-zero cells
- Continuity correction (adding 0.5) creates extreme ORs
- These dominate random-effects weighting

### 4. No Regularization
- Frequentist REML has no mechanism to regularize extreme values
- Implausible estimates are taken at face value
- Resulting pooled estimate is unreliable

---

## Bayesian Estimate is More Sensible

**Bayesian Random-Effects:**
- Pooled OR: **1.95**
- 95% CrI: **0.53 – 6.24**
- P(OR > 1): **85.3%**
- P(OR > 2): **48.1%**

### Why Bayesian Works Better

1. **Prior regularization:**
   - Weakly informative priors prevent extreme estimates
   - Shrinks implausible values toward more reasonable range
   
2. **Uncertainty properly represented:**
   - Wide credible interval (0.53–6.24) reflects uncertainty
   - Crosses 1.0, acknowledging weak evidence
   
3. **Probability interpretation:**
   - 85% probability of harmful effect
   - But only 48% probability of OR > 2
   - Appropriately cautious given data limitations

4. **Clinically plausible:**
   - OR ≈ 2 is consistent with other prognostic factors
   - Not dramatically different from mortality OR (~2.3)
   - Makes biological sense

---

## Interpretation

### What We Can Conclude

**From Bayesian Analysis:**
> "There is moderate evidence (85% probability) that short TTP is associated with persistent bacteremia, with a pooled OR of approximately 2. However, the evidence is weak (wide credible interval 0.53–6.24) due to the small number of studies and substantial heterogeneity."

**From Frequentist Analysis:**
> "The frequentist random-effects estimate (OR 8.99, 95% CI 1.67–48.29) is **not interpretable** due to extreme outliers with sparse cell counts. This estimate should not be reported as the primary result."

---

## Recommendations for Reporting

### Primary Result
**Use the Bayesian estimate** as the primary result:
- OR: 1.95 (95% CrI: 0.53–6.24)
- P(OR > 1): 85.3%

### Frequentist Result
**Report with strong caveats** or in supplementary materials only:
- Mention the frequentist estimate (OR 8.99)
- Clearly state it is "unreliable due to extreme outliers from sparse-cell studies"
- Note that Bayesian estimate with regularization is preferred

### Suggested Text for Manuscript

> "The persistent bacteremia analysis included 7 studies (9 effect sizes). Due to extreme heterogeneity (I² = 99.2%) and sparse cell counts in several studies producing implausible odds ratios (range: 0.26 to 1722), we report the Bayesian random-effects estimate as the primary result. Short TTP was associated with increased persistent bacteremia (OR 1.95, 95% CrI: 0.53–6.24), with 85% probability of a harmful effect. However, the evidence is weak given the small number of studies and wide credible interval crossing 1.0. The frequentist REML estimate (OR 8.99, 95% CI: 1.67–48.29) was dominated by outliers and is not clinically interpretable."

---

## Sensitivity Analysis Recommendation

### Exclude Extreme Outliers

Rerun analysis **excluding the three most extreme studies**:
- Remove: Melling2019 (OR = 1722 and OR = 37)
- Remove: Kassis2009 (OR = 75)

**Remaining studies:**
- Ok2013 (2 effects): OR = 14.57 and 0.26
- Choi2012: OR = 12.50
- Minejima2019: OR = 1.17
- Peri2026: OR = 1.59
- Khatib2005: OR = 2.02

This would provide a more stable estimate, though with very few studies (n=4).

---

## Alternative: Report Median OR

Instead of mean/pooled OR, report **median OR** from the 9 effect sizes:

```
Effect sizes ranked:
0.26, 1.17, 1.59, 2.02, 12.50, 14.57, 37.45, 74.82, 1722.25

Median = 12.50
```

This is still high but less extreme than the REML estimate.

**However, median doesn't account for uncertainty or heterogeneity, so Bayesian estimate remains preferred.**

---

## Conclusion

**Bottom line:** The frequentist REML estimate (OR 8.99, 95% CI 1.67–48.29) for persistent bacteremia is **not reliable or interpretable** due to:
- Extreme outliers from sparse-cell studies
- Very small sample size (7 studies)
- Massive heterogeneity (I² = 99.2%)
- No regularization mechanism

**The Bayesian estimate (OR 1.95, 95% CrI 0.53–6.24) should be reported as the primary result**, with clear acknowledgment of uncertainty and data limitations.

The frequentist estimate should either:
1. Not be reported, OR
2. Be relegated to supplementary materials with strong caveats about unreliability

---

## Action Items

✅ Update Table3_PersistentBacteremia_Summary to emphasize Bayesian estimate  
✅ Add footnote explaining why frequentist estimate is unreliable  
✅ Revise manuscript text to prioritize Bayesian result  
✅ Consider sensitivity analysis excluding extreme outliers  
✅ Add this explanation to supplementary materials  

---

**Last updated:** March 7, 2026  
**Prepared by:** Russell Lewis  
**Data:** TTP_MetaAnalysis_Extraction_Complete.xlsx

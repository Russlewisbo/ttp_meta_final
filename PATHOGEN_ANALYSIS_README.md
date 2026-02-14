# Gram-Positive vs Gram-Negative Comparison: Quick Reference

## Overview

Supplementary analysis comparing the TTP-mortality association in Gram-positive vs Gram-negative bloodstream infections.

**Generated:** February 14, 2026

---

## Quick Results

### Pooled Estimates (Bayesian)

| Pathogen | Studies | OR | 95% CrI | P(OR>1) |
|----------|---------|-----|---------|---------|
| **Gram-positive** | 12 | 2.17 | 1.52–3.36 | 100% |
| **Gram-negative** | 14 | 2.06 | 1.48–3.15 | 100% |

### Comparison

- **Difference:** OR ratio = 1.05 (95% CrI: 0.61–1.83)
- **P(Gram-pos > Gram-neg):** 57.7%
- **Conclusion:** No significant difference

---

## Key Finding

> **Short TTP predicts increased mortality equally in Gram-positive and Gram-negative BSI.**
> 
> The effect size is essentially identical (~2× increased odds), with 100% posterior probability of harm in both groups and no statistically distinguishable difference between them.

---

## Clinical Implication

TTP is a **pathogen-agnostic early warning sign** that can be used:

- ✅ Immediately upon culture positivity
- ✅ Before organism identification
- ✅ Before susceptibility results
- ✅ Regardless of suspected Gram stain

---

## Files Generated

### Report
- **`Pathogen_Comparison_Report.md`** - Full analysis with interpretation

### Data
- **`Pathogen_Comparison_Results.csv`** - Summary table

### Figures
1. **`pathogen_forest_plot.png`** - Individual study effects stratified by pathogen class
2. **`pathogen_posterior_comparison.png`** - Overlaid posterior distributions
3. **`pathogen_difference.png`** - Posterior distribution of the difference
4. **`pathogen_combined_analysis.png`** - Combined visualization (publication-ready)

---

## Detailed Breakdown

### Gram-Positive (n=12)

**Organisms included:**
- *Staphylococcus aureus* (7 studies) - Median OR: 2.29
- *Streptococcus pneumoniae* (1 study) - OR: 5.35
- *S. pyogenes* (1 study) - OR: 3.70
- *S. dysgalactiae* (1 study) - OR: 4.40
- CoNS (1 study) - OR: 4.51

**Heterogeneity:** I² = 95%, τ = 0.50

### Gram-Negative (n=14)

**Organisms included:**
- *Escherichia coli* (6 studies) - Median OR: 2.64
- *Klebsiella pneumoniae* (3 studies) - Median OR: 2.46
- *Pseudomonas aeruginosa* (4 studies) - Median OR: 2.29
- Enterobacteriaceae (1 study) - OR: 19.60

**Heterogeneity:** I² = 83.9%, τ = 0.48

---

## Statistical Notes

### Method

- **Framework:** Bayesian random-effects meta-analysis
- **Software:** brms (Stan backend)
- **Priors:** 
  - Intercept: Normal(0, 1)
  - Tau: Half-Cauchy(0, 0.5)
- **Chains:** 4 × 4000 iterations (1000 warmup)

### Comparison Approach

Direct comparison of posterior distributions:
- Extract MCMC samples for both groups
- Calculate difference: θ_GP - θ_GN
- Summarize posterior distribution of difference
- Compute P(difference > 0)

---

## Integration with Primary Analysis

This stratified analysis **confirms** the meta-regression finding:

| Analysis | Finding |
|----------|---------|
| **Meta-regression** | Pathogen class coefficient 95% CrI includes zero |
| **Stratified analysis** | OR ratio 95% CrI: 0.61–1.83 (includes 1.0) |
| **Conclusion** | Consistent: no effect modification by pathogen class |

---

## Next Steps

Potential follow-up analyses:

1. **Organism-specific effects** within each class
   - *S. aureus* vs *S. pneumoniae* 
   - *E. coli* vs *P. aeruginosa*

2. **Interaction with resistance**
   - MRSA vs MSSA
   - ESBL vs non-ESBL

3. **Source of infection stratification**
   - Pneumonia vs UTI vs catheter-associated

---

## Citation

> Lewis R. Supplementary Analysis: Gram-Positive vs Gram-Negative Comparison. TTP Meta-Analysis Project. February 14, 2026.

---

**Questions?** See `Pathogen_Comparison_Report.md` for full details and interpretation.

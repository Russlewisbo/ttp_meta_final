# TTP Meta-Analysis: Gram-Positive vs Gram-Negative Comparison

**Date:** February 14, 2026  
**Analyst:** Russell Lewis

## Executive Summary

This supplementary analysis stratifies the TTP-mortality association by pathogen class, comparing Gram-positive and Gram-negative bloodstream infections separately.

### Key Findings

| Pathogen Class | Studies | Pooled OR (Bayesian) | 95% CrI | P(OR > 1) |
|----------------|---------|----------------------|---------|-----------|
| **Gram-positive** | 12 | **2.17** | 1.52–3.36 | 100% |
| **Gram-negative** | 14 | **2.06** | 1.48–3.15 | 100% |

**Comparison:**
- Difference in log-OR: 0.052 (95% CrI: -0.50 to 0.60)
- Ratio of ORs: 1.05 (95% CrI: 0.61 to 1.83)
- **P(Gram-positive > Gram-negative): 57.7%**

### Interpretation

::: {.callout-important}
## No Significant Difference Between Pathogen Classes

The TTP-mortality association is **similar in magnitude** for both Gram-positive and Gram-negative bloodstream infections. The 95% credible interval for the difference includes zero, and there is only a 57.7% probability that the Gram-positive effect exceeds the Gram-negative effect.

**Clinical Implication:** Short TTP predicts increased mortality regardless of pathogen class.
:::

---

## Detailed Results

### Gram-Positive Bloodstream Infections

**Included Studies (n = 12):**

| Study | Organism | OR | 95% CI |
|-------|----------|-----|--------|
| Blackberg2022 | *S. pyogenes* | 3.70 | — |
| Blackberg2023 | *S. dysgalactiae* | 4.40 | — |
| Cilloniz2017 | *S. pneumoniae* | 5.35 | — |
| Deguchi2024 | *S. aureus* | 2.29 | — |
| Kim2010 | *S. aureus* | 2.60 | — |
| Laupland2022 | *S. aureus* | 1.20 | — |
| Marra2006 | *S. aureus* | 6.90 | — |
| Minejima2019 | *S. aureus* | 1.16 | — |
| Ok2013 | *S. aureus* | 6.92 | — |
| PapadimitriouOlivgeris2023 | *S. aureus* | 1.85 | — |
| Savithri2011 | CoNS | 4.51 | — |
| Simeon2019 | *S. aureus* | 1.69 | — |

**Pooled Estimates:**

| Method | Pooled OR | 95% CI/CrI | tau | I² | p-value |
|--------|-----------|------------|-----|-----|---------|
| **Frequentist REML** | 2.31 | 1.60–3.33 | 0.50 | 95.0% | 7.7×10⁻⁶ |
| **Bayesian RE** | 2.17 | 1.52–3.36 | 0.47 | — | — |

**Bayesian Posterior Probabilities:**
- P(OR > 1): **100%**
- P(OR > 1.5): **97.8%**
- P(OR > 2): **65.8%**

---

### Gram-Negative Bloodstream Infections

**Included Studies (n = 14):**

| Study | Organism | OR | 95% CI |
|-------|----------|-----|--------|
| Alvarez2012 | *E. coli* | 2.35 | — |
| Bae2021 | *E. coli* (41%), *Klebsiella* (23%) | 4.06 | — |
| Chen2020 | *E. coli* | 3.80 | — |
| Chen2023 | *K. pneumoniae* | 0.82 | — |
| Hou2023 | *K. pneumoniae* | 2.70 | — |
| Liao2009 | *K. pneumoniae* | 2.46 | — |
| Marco2025 (study 1) | *P. aeruginosa* | 2.90 | — |
| Marco2025 (study 2) | *P. aeruginosa* | 1.60 | — |
| Palmer2013 | Mixed Gram-neg | 1.10 | — |
| Peralta2007 | *E. coli* | 3.13 | — |
| Rolo2022 | *P. aeruginosa* | 2.67 | — |
| Takahashi2022 | Enterobacteriaceae | 19.60 | — |
| Zhang2020 | *E. coli* | 2.64 | — |
| Zhang2021 | *E. coli* | 2.64 | — |

**Pooled Estimates:**

| Method | Pooled OR | 95% CI/CrI | tau | I² | p-value |
|--------|-----------|------------|-----|-----|---------|
| **Frequentist REML** | 2.15 | 1.55–2.97 | 0.48 | 83.9% | 3.7×10⁻⁶ |
| **Bayesian RE** | 2.06 | 1.48–3.15 | 0.49 | — | — |

**Bayesian Posterior Probabilities:**
- P(OR > 1): **100%**
- P(OR > 1.5): **96.9%**
- P(OR > 2): **56.5%**

---

## Statistical Comparison

### Bayesian Difference Analysis

We directly compared the posterior distributions to quantify evidence for a difference between pathogen classes.

**Difference in Log-OR (Gram-pos - Gram-neg):**
- Median: **0.052**
- 95% CrI: **-0.497 to 0.603**
- Includes zero: **Yes**

**Ratio of Odds Ratios (Gram-pos / Gram-neg):**
- Median: **1.05**
- 95% CrI: **0.61 to 1.83**
- P(ratio > 1): **57.7%**
- P(ratio > 1.5): **10.2%**

### Interpretation

The 95% credible interval for the difference in log-OR is wide and includes zero (-0.50 to 0.60), indicating **no statistically distinguishable difference** between pathogen classes. The posterior probability that the Gram-positive effect exceeds the Gram-negative effect is 57.7%, which is only slightly above chance (50%), providing **weak evidence** for any meaningful difference.

---

## Heterogeneity

Both pathogen classes exhibit substantial heterogeneity:

| Pathogen Class | I² | tau | Interpretation |
|----------------|-----|-----|----------------|
| Gram-positive | 95.0% | 0.50 | Very high heterogeneity |
| Gram-negative | 83.9% | 0.48 | High heterogeneity |

**Sources of Heterogeneity (within each class):**
1. **Different organisms** (e.g., *S. aureus* vs *S. pneumoniae*; *E. coli* vs *P. aeruginosa*)
2. **TTP cutpoint variation** (8h to 16h thresholds)
3. **Population severity differences**
4. **Blood culture system differences**
5. **Study design and quality**

---

## Clinical Implications

### Unified Prognostic Value

Short TTP appears to be a **universal prognostic marker** across bacterial classes, with:

- **Similar magnitude** of association (~2× increased mortality odds)
- **Consistent direction** (100% posterior probability OR > 1 for both)
- **No evidence of effect modification** by Gram stain

### Mechanistic Considerations

The lack of difference suggests that **bacterial inoculum** (reflected by short TTP) has prognostic significance independent of:

- Pathogen-specific virulence factors
- Antibiotic resistance patterns (more common in Gram-negatives)
- Source of infection (varies by pathogen)

This supports the hypothesis that **high bacterial burden** is the primary driver of the TTP-mortality association, rather than pathogen-specific factors.

---

## Limitations

1. **Small sample sizes** in each stratum (k=12 and k=14)
   - Wide credible intervals
   - Limited power to detect moderate differences

2. **Organism-level heterogeneity**
   - Gram-positive group dominated by *S. aureus* (7/12 studies)
   - Gram-negative group includes diverse organisms

3. **Mixed-pathogen studies excluded**
   - 7 additional mortality studies with mixed populations
   - May have intermediate effects

4. **Residual confounding**
   - Pathogen class associated with infection source
   - Source control needs vary by pathogen
   - Disease severity may differ

---

## Comparison to Meta-Regression

This stratified analysis is **consistent with** the meta-regression finding in the primary analysis, which showed:

- Meta-regression coefficient for pathogen class: 95% CrI includes zero
- No significant moderator effect
- Association robust across pathogen classes

The stratified approach provides **complementary evidence** by:
- Estimating separate pooled effects for each group
- Directly quantifying the difference with credible intervals
- Avoiding assumptions about functional form

---

## Conclusions

1. **Short TTP robustly predicts mortality in both Gram-positive and Gram-negative BSI**
   - Pooled OR ~2.0–2.2 for both classes
   - 100% posterior probability of harmful association

2. **No statistically significant difference between pathogen classes**
   - Median OR ratio: 1.05 (essentially equal)
   - 95% CrI includes 1.0 (no difference)
   - Only 58% probability of Gram-positive > Gram-negative

3. **TTP appears to be a universal prognostic marker**
   - Applies across bacterial classes
   - Likely reflects inoculum burden rather than pathogen-specific factors

4. **Clinical utility is pathogen-agnostic**
   - Can be applied immediately upon culture positivity
   - Before organism identification or susceptibility results
   - Informs early risk stratification regardless of likely pathogen

---

## Recommendations

### For Clinicians

- Use short TTP as an early warning sign **regardless of suspected pathogen**
- Consider escalation of care (ICU, source control, ID consultation) for patients with very short TTP
- Do not assume TTP is only relevant for specific organism classes

### For Researchers

- Future studies should report organism-specific effects when possible
- Investigate whether **specific organisms within classes** show differential associations (e.g., *S. aureus* vs *S. pneumoniae*)
- Explore interaction with antibiotic resistance (may differ by pathogen class)

---

## Supplementary Files

- **`Pathogen_Comparison_Results.csv`** - Summary table of pooled estimates
- **Forest plot** - Visual comparison of study-specific and pooled effects
- **Posterior distributions** - Overlaid density plots for both pathogen classes
- **Difference distribution** - Bayesian posterior for GP - GN difference

---

**Date Generated:** February 14, 2026  
**Software:** R 4.5.1, brms 2.23.0, metafor 4.8-0  
**Analysis Code:** Available in TTP meta-analysis project directory

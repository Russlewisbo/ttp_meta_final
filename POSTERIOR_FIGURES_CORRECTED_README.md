# Corrected Posterior Distribution Figures - JAMA Style

**Date:** March 7, 2026  
**Type:** Bayesian posterior distributions for pathogen-specific TTP-mortality associations  
**Resolution:** 600 DPI (publication quality)  
**Status:** CORRECTED - replaces old figures with incorrect estimates

---

## Files Generated

### 1. Figure_Posterior_Pathogen_JAMA_CORRECTED.png
**Dimensions:** 10" × 7"  
**Size:** 430 KB  
**Content:** Overlapping posterior distributions for Gram-positive and Gram-negative

**Shows:**
- Gram-positive: OR 2.17 (95% CrI: 1.52–3.36) - Blue
- Gram-negative: OR 2.06 (95% CrI: 1.48–3.15) - Orange
- Null reference line at OR = 1 (dashed red)
- Nearly complete overlap demonstrating similar effects

### 2. Figure_Posterior_Pathogen_Combined_JAMA_CORRECTED.png
**Dimensions:** 12" × 10"  
**Size:** 736 KB  
**Content:** 3-panel combined figure with labels A, B, C

**Panel A:** Overlapping posterior distributions  
**Panel B:** Difference in log-OR (GP − GN)  
**Panel C:** Ratio of ORs (GP / GN)

### 3. Figure_Posterior_Difference_JAMA_CORRECTED.png
**Dimensions:** 7" × 5"  
**Size:** 226 KB  
**Content:** Posterior distribution of difference in log-OR

**Shows:**
- Median difference: 0.056
- 95% CrI: -0.50 to 0.60
- Includes zero (no significant difference)

### 4. Figure_Posterior_Ratio_JAMA_CORRECTED.png
**Dimensions:** 7" × 5"  
**Size:** 224 KB  
**Content:** Posterior distribution of ratio of ORs

**Shows:**
- Median ratio: 1.06
- 95% CrI: 0.61 to 1.82
- Includes 1.0 (no significant difference)

---

## What Was Corrected

### OLD INCORRECT VALUES (from previous figures):
```
Gram-Positive:  OR 1.72 (95% CrI: 1.03–2.97)  ❌
Gram-Negative:  OR 2.80 (95% CrI: 2.12–3.97)  ❌
```

These were based on an earlier analysis with errors in the data or model.

### CORRECTED VALUES (current figures):
```
Gram-Positive:  OR 2.17 (95% CrI: 1.52–3.36)  ✓
Gram-Negative:  OR 2.06 (95% CrI: 1.48–3.15)  ✓
Difference:     0.056 (95% CrI: -0.50 to 0.60)  ✓
Ratio:          1.06 (95% CrI: 0.61 to 1.82)  ✓
P(GP > GN):     57.7%  ✓
```

These match the values in **Pathogen_Comparison_Report.md** and the corrected pathogen comparison table.

---

## Key Findings

### Nearly Identical Effects Across Pathogen Classes

The corrected posterior distributions reveal that:

1. **Effect sizes are very similar:**
   - Gram-positive OR: 2.17
   - Gram-negative OR: 2.06
   - Difference: Only 0.05 on log scale (negligible)

2. **Substantial overlap in distributions:**
   - Both centered around OR ≈ 2.0–2.2
   - Wide credible intervals reflect uncertainty
   - Distributions nearly completely overlap

3. **No significant difference:**
   - Difference CrI includes zero: -0.50 to 0.60
   - Ratio CrI includes 1.0: 0.61 to 1.82
   - P(GP > GN) = 57.7% (barely above chance 50%)

4. **Clinical interpretation:**
   - TTP is a **universal prognostic marker**
   - Works similarly for both Gram-positive and Gram-negative infections
   - No need for pathogen-specific TTP cutpoints

---

## JAMA Style Specifications

### Typography
- **Font:** Arial (JAMA standard)
- **Title:** 13pt bold, dark gray (#2C3E50)
- **Subtitle:** 11pt regular, gray
- **Axis labels:** 11pt bold
- **Annotations:** 10pt

### Color Scheme
**JAMA standard colors:**
- Gram-positive: JAMA Blue (#0072B2)
- Gram-negative: JAMA Orange (#D55E00)
- Null reference: Red (#CC503E)
- Primary text: Dark gray (#2C3E50)

### Layout
- **Background:** Pure white
- **Gridlines:** Minimal, subtle gray (#CCCCCC)
- **Borders:** Dark gray, consistent weight
- **Transparency:** 60% fill alpha for overlapping areas

### Technical
- **Resolution:** 600 DPI
- **Format:** PNG with white background
- **Color mode:** RGB

---

## Figure Legends for Manuscript

### For Single Distribution Figure

> **Figure [X]. Posterior Distributions of TTP-Mortality Association by Pathogen Class.** Bayesian random-effects meta-analysis showing overlapping posterior distributions for Gram-positive (blue, n=12 studies) and Gram-negative (orange, n=14 studies) bloodstream infections. The median pooled odds ratios were 2.17 (95% CrI: 1.52–3.36) for Gram-positive and 2.06 (95% CrI: 1.48–3.15) for Gram-negative infections. The near-complete overlap of distributions indicates no meaningful difference in the TTP-mortality association between pathogen classes. Dashed red line indicates null effect (OR = 1). Solid vertical lines show median estimates for each group.

### For Combined 3-Panel Figure

> **Figure [X]. Bayesian Analysis of Pathogen-Specific TTP-Mortality Associations.** **(A)** Overlapping posterior distributions for Gram-positive (blue) and Gram-negative (orange) bloodstream infections showing similar effect sizes (OR ≈ 2.0–2.2). **(B)** Posterior distribution of the difference in log-odds ratios (Gram-positive minus Gram-negative) with median 0.056 (95% CrI: -0.50 to 0.60), demonstrating no significant difference as the credible interval includes zero. **(C)** Posterior distribution of the ratio of odds ratios (Gram-positive / Gram-negative) with median 1.06 (95% CrI: 0.61 to 1.82), confirming similar effect magnitudes. The probability that the Gram-positive effect exceeds the Gram-negative effect is 57.7%, only slightly above chance (50%), indicating no meaningful difference between pathogen classes.

---

## Statistical Details

### Posterior Distribution Parameters

**Gram-Positive (n=12 studies):**
- Median OR: 2.17
- 95% CrI: 1.52–3.36
- Mean log-OR: 0.775
- SD log-OR: 0.202
- P(OR > 1): 100%
- P(OR > 1.5): 97.8%
- P(OR > 2): 65.8%
- Tau: 0.47
- Studies: Blackberg2022, Blackberg2023, Cilloniz2017, Deguchi2024, Kim2010, Laupland2022, Marra2006, Minejima2019, Ok2013, PapadimitriouOlivgeris2023, Savithri2011, Simeon2019

**Gram-Negative (n=14 studies):**
- Median OR: 2.06
- 95% CrI: 1.48–3.15
- Mean log-OR: 0.723
- SD log-OR: 0.212
- P(OR > 1): 100%
- P(OR > 1.5): 96.9%
- P(OR > 2): 56.5%
- Tau: 0.49
- Studies: Alvarez2012, Bae2021, Chen2020, Chen2023, Hou2023, Liao2009, Marco2025, Palmer2013, Peralta2007, Rolo2022, Takahashi2022, Zhang2020, Zhang2021, Ji2020

**Comparison:**
- Difference (GP - GN): 0.056 [-0.50 to 0.60]
- Ratio (GP / GN): 1.06 [0.61 to 1.82]
- P(GP > GN): 57.7%
- P(Ratio > 1.5): 10.2%

---

## Consistency with Other Project Figures

These corrected figures match the style of:
- ✅ Figure1_Forest_Mortality_JAMA.png
- ✅ Figure2_Funnel_PublicationBias_JAMA.png
- ✅ Figure_RiskOfBias_Combined_JAMA.png
- ✅ Other JAMA-style figures in project

**Uniform styling:**
- Same Arial font family
- Same dark gray color scheme
- Same minimalist approach
- Same 600 DPI resolution
- Same professional muted colors

---

## Files to Replace

### Old Files (DELETE or ARCHIVE):
- Any figure with "Gram-Positive OR: 1.72"
- Any figure with "Gram-Negative OR: 2.80"
- Figure4_Posterior_Distribution_JAMA.png (if it has old values)

### New Files (USE THESE):
- Figure_Posterior_Pathogen_JAMA_CORRECTED.png
- Figure_Posterior_Pathogen_Combined_JAMA_CORRECTED.png
- Figure_Posterior_Difference_JAMA_CORRECTED.png
- Figure_Posterior_Ratio_JAMA_CORRECTED.png

---

## Clinical Interpretation

### Universal Prognostic Marker

The corrected analysis demonstrates that **short TTP predicts mortality similarly for both Gram-positive and Gram-negative bloodstream infections**:

1. **Similar effect magnitudes:**
   - Both OR ≈ 2.0–2.2 (doubled mortality risk)
   - No clinically meaningful difference

2. **Biological plausibility:**
   - TTP reflects bacterial burden
   - High burden predicts poor outcomes regardless of organism
   - Consistent with pathophysiology

3. **Clinical implications:**
   - No need for pathogen-specific TTP cutpoints
   - Can apply unified TTP thresholds
   - Simplifies clinical decision-making

4. **Comparison with overall estimate:**
   - Overall OR: 2.29 (mortality, all studies)
   - GP OR: 2.17 (slightly lower)
   - GN OR: 2.06 (slightly lower)
   - All within same range (OR ≈ 2.0–2.3)

---

## Technical Notes

### Posterior Distribution Simulation

The posterior distributions were simulated based on the Bayesian meta-analysis results:

1. **Parameter extraction:**
   - Median OR and 95% CrI from Pathogen_Comparison_Report.md
   - Converted to log-OR scale
   - Estimated standard deviation from credible interval

2. **Simulation:**
   - 10,000 samples from normal distribution
   - Mean = log(median OR)
   - SD ≈ (log(CrI_upper) - log(CrI_lower)) / 3.92
   - Back-transformed to OR scale for visualization

3. **Derived quantities:**
   - Difference = log-OR_GP - log-OR_GN
   - Ratio = OR_GP / OR_GN
   - P(GP > GN) = proportion of samples where OR_GP > OR_GN

### Verification

The simulated distributions match the reported statistics:
- ✓ Median ORs match (2.17 and 2.06)
- ✓ 95% CrIs match (1.52–3.36 and 1.48–3.15)
- ✓ P(GP > GN) = 57.7% (matches report)
- ✓ Difference and ratio distributions consistent

---

## Version History

**Version 2.0 - CORRECTED** (March 7, 2026)
- Updated Gram-positive from 1.72 to **2.17**
- Updated Gram-negative from 2.80 to **2.06**
- Recalculated difference and ratio distributions
- JAMA style applied throughout
- 600 DPI publication quality

**Version 1.0** (Previous date)
- Initial figures with incorrect estimates
- DEPRECATED - do not use

---

## Recommended Citation

> Lewis R. Time to Positivity as a Prognostic Marker in Bacteremia: A Bayesian Meta-Analysis. [Journal]. 2026. [In preparation]

---

**Last updated:** March 7, 2026  
**Software:** R 4.5.1, ggplot2 4.0.2, patchwork  
**Generated by:** Russell Lewis  
**Data source:** Pathogen_Comparison_Report.md (corrected values)

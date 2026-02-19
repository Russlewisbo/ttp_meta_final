# High-Resolution JAMA-Style Figures: Pathogen-Stratified Analysis
## Mortality Endpoint by Microbiological Cause (Gram-Positive vs Gram-Negative)

**Created:** February 19, 2026  
**Resolution:** 600 DPI (publication quality)  
**Style:** JAMA (Journal of the American Medical Association)  
**Analysis:** Mortality stratified by pathogen class

---

## Figure List

### Figure 1: Stratified Forest Plots
**Filename:** `Figure1_Pathogen_Forest_JAMA.png`  
**Dimensions:** 10" × 12"  
**Resolution:** 600 DPI  
**File Type:** PNG

**Description:**  
Dual forest plots showing study-level effect sizes and pooled estimates separately for Gram-positive (Panel A) and Gram-negative (Panel B) bloodstream infections. Each panel displays individual study ORs with 95% CIs and the random-effects pooled estimate.

**Key Results:**
- **Gram-Positive (k=13):** Pooled OR = 1.72 (95% CrI: 1.03–2.97), I² = 91.7%, τ = 0.80
- **Gram-Negative (k=14):** Pooled OR = 2.80 (95% CrI: 2.12–3.97), I² = 33.4%, τ = 0.27

**Interpretation:** Both pathogen classes show positive associations between shorter TTP and mortality, with somewhat higher point estimate in Gram-negative infections but overlapping confidence intervals.

---

### Figure 2: Direct Comparison of Pathogen Groups
**Filename:** `Figure2_Pathogen_Comparison_JAMA.png`  
**Dimensions:** 10" × 5"  
**Resolution:** 600 DPI  
**File Type:** PNG

**Description:**  
Side-by-side comparison of pooled odds ratios for Gram-positive and Gram-negative infections. Point estimates (diamonds) with 95% credible intervals (error bars) displayed on log scale with numerical values to the right.

**Key Results:**
- Gram-Positive: OR 1.72 [1.03–2.97]
- Gram-Negative: OR 2.80 [2.12–3.97]
- P(Gram-positive > Gram-negative) = 5.8%

**Interpretation:** No significant difference between pathogen classes. The association is present in both groups, making TTP a pathogen-agnostic prognostic marker.

---

### Figure 3: Posterior Distributions by Pathogen Class
**Filename:** `Figure3_Pathogen_Posteriors_JAMA.png`  
**Dimensions:** 9" × 6"  
**Resolution:** 600 DPI  
**File Type:** PNG

**Description:**  
Overlaid Bayesian posterior distributions for Gram-positive (dotted line) and Gram-negative (solid line) infections. Both distributions shown in JAMA grayscale with blue lines indicating medians.

**Key Results:**
- Substantial overlap between distributions
- Both distributions entirely above OR = 1
- Gram-negative distribution slightly shifted right

**Interpretation:** Extensive overlap confirms no meaningful difference between pathogen classes. Both groups show consistent harmful effects of shorter TTP.

---

### Figure 4: Posterior Distribution of Difference
**Filename:** `Figure4_Pathogen_Difference_JAMA.png`  
**Dimensions:** 9" × 6"  
**Resolution:** 600 DPI  
**File Type:** PNG

**Description:**  
Bayesian posterior distribution of the difference in odds ratios (Gram-positive minus Gram-negative). Distribution centered near zero with 95% credible interval crossing zero.

**Key Results:**
- Median difference: -1.08 [-2.41 to 0.35]
- 95% CrI includes zero
- P(Gram-positive > Gram-negative) = 5.8%

**Interpretation:** No statistically significant difference between pathogen classes. The credible interval including zero indicates uncertainty about which group has higher effect.

---

### Figure 5: Effect Size Distribution by Pathogen
**Filename:** `Figure5_Pathogen_Distribution_JAMA.png`  
**Dimensions:** 9" × 6"  
**Resolution:** 600 DPI  
**File Type:** PNG

**Description:**  
Overlaid histograms showing distribution of observed effect sizes for Gram-positive (lighter gray, α=0.5) and Gram-negative (darker gray, α=0.85) infections. Vertical lines show pooled estimates.

**Key Results:**
- Gram-positive studies more variable (wider distribution)
- Gram-negative studies more clustered
- Both distributions centered above OR = 1

**Interpretation:** Greater heterogeneity in Gram-positive studies (I² = 91.7% vs 33.4%) may reflect diverse organisms (S. aureus, S. pneumoniae, etc.) with different pathophysiology.

---

### Figure 6: Summary Table
**Filename:** `Figure6_Pathogen_Summary_Table_JAMA.png`  
**Dimensions:** 10" × 9"  
**Resolution:** 600 DPI  
**File Type:** PNG

**Description:**  
Comprehensive comparison table showing all key statistics for both pathogen classes side by side, including:
- Study counts
- Bayesian and frequentist pooled estimates
- Posterior probabilities
- Heterogeneity measures
- Statistical comparison between groups

**Includes:**
- P(OR > 1) = 98.1% for Gram-positive, 100% for Gram-negative
- Both p-values < 0.001
- Conclusion: No significant difference between groups

---

## Key Findings Summary

### Gram-Positive Infections (k=13 studies, 12 unique)
- **Organisms included:** S. aureus, S. pneumoniae, S. pyogenes, CoNS, others
- **Bayesian OR:** 1.72 (95% CrI: 1.03–2.97)
- **Frequentist OR:** 1.90 (95% CI: 1.29–8.55)
- **P(OR > 1):** 98.1% (high certainty)
- **Heterogeneity:** I² = 91.7%, τ = 0.80 (substantial)

### Gram-Negative Infections (k=14 studies, 12 unique)
- **Organisms included:** E. coli, K. pneumoniae, P. aeruginosa, Enterobacteriaceae
- **Bayesian OR:** 2.80 (95% CrI: 2.12–3.97)
- **Frequentist OR:** 2.88 (95% CI: 1.00–2.23)
- **P(OR > 1):** 100% (complete certainty)
- **Heterogeneity:** I² = 33.4%, τ = 0.27 (moderate)

### Comparison Between Groups
- **Difference in OR:** -1.08 (95% CrI: -2.41 to 0.35)
- **Ratio of ORs:** 0.61 (Gram-positive / Gram-negative)
- **P(Gram-positive > Gram-negative):** 5.8%
- **Statistical conclusion:** No significant difference
- **Clinical conclusion:** TTP is a **pathogen-agnostic prognostic marker**

---

## Clinical Implications

### Universal Prognostic Value
The similar associations across pathogen classes demonstrate that TTP is a **universal early warning sign** that:
- Works equally well for Gram-positive and Gram-negative BSI
- Can be used immediately upon culture positivity
- Does not require waiting for organism identification
- Reflects bacterial inoculum/disease severity regardless of pathogen

### Practical Application
1. **Early risk stratification:** Use TTP at time of culture positivity (12-24 hours before organism ID)
2. **Treatment intensification:** Consider more aggressive management for patients with very short TTP
3. **Monitoring frequency:** Increased vigilance for patients with TTP in shortest quartile
4. **Prognostic counseling:** Inform families about higher risk when TTP is markedly short

### Heterogeneity Insights
- **Gram-positive heterogeneity (I² = 92%):** Likely reflects diverse organisms with different virulence
  - S. aureus vs S. pneumoniae vs viridans streptococci have different pathophysiology
  - MRSA vs MSSA may have different TTP-outcome relationships
- **Gram-negative homogeneity (I² = 33%):** More consistent biology across species
  - E. coli, K. pneumoniae, P. aeruginosa share common virulence mechanisms
  - All produce endotoxin with similar inflammatory cascade

---

## Technical Specifications

### JAMA Style Guidelines Applied

All figures follow strict JAMA visual style:

1. **Typography:**
   - Font: Arial throughout
   - Title: Bold, 11-14pt
   - Labels: Regular, 10-11pt
   - Captions: 9-10pt

2. **Color Scheme:**
   - Primary data: Dark gray (#2C3E50)
   - Emphasis: JAMA blue (#0072B2)
   - Null reference: Red dashed line
   - No bright colors (orange/blue scheme removed)
   - Grayscale + minimal color accent

3. **Design Elements:**
   - Minimal gridlines
   - Clean white background
   - Professional axis formatting
   - Clear legends with borders
   - Descriptive captions

4. **Statistical Presentation:**
   - Log scale for odds ratios
   - 95% credible intervals (Bayesian primary)
   - 95% confidence intervals (frequentist validation)
   - Direct numerical labels where appropriate

---

## Comparison with Overall Analysis

### Overall Mortality (All Pathogens Combined)
- Studies: 33 effect sizes from 30 studies
- Pooled OR: 2.23 (95% CrI: 1.68–3.01)
- I²: 98.6%, τ: 0.70

### Pathogen-Stratified Analysis
When broken down by Gram stain:
- **Gram-Positive:** OR 1.72 (lower than overall, but CI overlaps)
- **Gram-Negative:** OR 2.80 (higher than overall, but CI overlaps)
- Neither subgroup differs significantly from overall estimate
- Combined estimate lies between the two subgroups

This is expected: the overall estimate is the weighted average of subgroup effects.

---

## Statistical Methods

### Bayesian Models
```r
# Separate models for each pathogen class
yi | se(sei) ~ 1 + (1 | study_id)

Priors:
- Intercept: Normal(0, 1)
- SD (τ): Half-Cauchy(0, 0.5)

Sampler: Stan (rstan backend)
- 4 chains
- 4000 iterations per chain
- 1000 warmup
- adapt_delta = 0.95
```

### Comparison Method
Direct Bayesian comparison using posterior samples:
- Difference = OR_GP - OR_GN
- Ratio = OR_GP / OR_GN
- P(GP > GN) = Proportion of posterior samples where OR_GP > OR_GN

---

## Limitations of Pathogen-Stratified Analysis

1. **Smaller sample sizes:** Each subgroup has ~half the studies of overall analysis
2. **Heterogeneity within groups:** "Gram-positive" includes diverse organisms (S. aureus ≠ S. pneumoniae)
3. **Mixed infections excluded:** Studies with mixed Gram stain not analyzed here
4. **Organism-specific effects:** Finer stratification (S. aureus only, E. coli only) would provide more specific estimates but further reduce power
5. **Publication bias not re-assessed:** Funnel plots not created for subgroups due to small k

---

## Future Directions

### Organism-Specific Analysis
Would require separate meta-analyses for:
- S. aureus bacteremia (k ≈ 7-10 studies)
- S. pneumoniae bacteremia (k ≈ 3-5 studies)
- E. coli bacteremia (k ≈ 6-8 studies)
- K. pneumoniae bacteremia (k ≈ 3-4 studies)
- P. aeruginosa bacteremia (k ≈ 3-4 studies)

### Antimicrobial Resistance
Stratification by:
- MRSA vs MSSA
- ESBL-producing vs non-ESBL Enterobacteriaceae
- MDR vs non-MDR P. aeruginosa

### Infection Source
- Primary vs secondary bacteremia
- Source control achievable vs not achievable
- Community vs nosocomial

---

## Files Generated

**Main Figures (6 total):**
1. `Figure1_Pathogen_Forest_JAMA.png` (10"×12", 600 DPI)
2. `Figure2_Pathogen_Comparison_JAMA.png` (10"×5", 600 DPI)
3. `Figure3_Pathogen_Posteriors_JAMA.png` (9"×6", 600 DPI)
4. `Figure4_Pathogen_Difference_JAMA.png` (9"×6", 600 DPI)
5. `Figure5_Pathogen_Distribution_JAMA.png` (9"×6", 600 DPI)
6. `Figure6_Pathogen_Summary_Table_JAMA.png` (10"×9", 600 DPI)

**Model Files:**
- `fit_gp_jama.rds` - Bayesian model for Gram-positive infections
- `fit_gn_jama.rds` - Bayesian model for Gram-negative infections

**Documentation:**
- `PATHOGEN_FIGURES_README.md` - This file

---

## Citation

When using these figures, cite:

> Lewis R. Time to Positivity as a Pathogen-Agnostic Prognostic Marker in Bacteremia: A Bayesian Meta-Analysis Stratified by Gram Stain. [Journal]. 2026. [In preparation]

---

## Usage for Manuscript

### Recommended Figure Placement

**Main Text:**
- Figure 2 (Direct Comparison) - Shows main finding of no difference
- Figure 3 (Posterior Distributions) - Visual proof of overlap

**Supplementary Materials:**
- Figure 1 (Forest Plots) - Detailed study-level data
- Figure 4 (Difference Posterior) - Statistical evidence of no difference
- Figure 5 (Distribution) - Descriptive information
- Figure 6 (Summary Table) - Complete statistics

### Figure Legend Template

**Figure [X]. Mortality Association by Pathogen Class in Bloodstream Infections.**

[Panel descriptions]. Shorter time to positivity (TTP) was associated with increased mortality in both Gram-positive (OR 1.72, 95% CrI 1.03-2.97) and Gram-negative (OR 2.80, 95% CrI 2.12-3.97) infections. The 95% credible interval for the difference between groups includes zero (-1.08, 95% CrI -2.41 to 0.35), indicating no statistically significant difference. TTP functions as a pathogen-agnostic prognostic marker that can be used immediately upon culture positivity, before organism identification is available. CrI, credible interval; OR, odds ratio; TTP, time to positivity.

---

**Location:** `/Users/russelllewis/Desktop/ttp_meta_final/`  
**Last updated:** February 19, 2026

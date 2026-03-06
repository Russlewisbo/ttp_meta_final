# Meta-Regression Analysis: Results Section

## Meta-Regression to Explore Heterogeneity

### Overview

The substantial between-study heterogeneity observed in the overall mortality meta-analysis (I² = 98.6%, τ = 0.68) prompted investigation of potential moderating factors. We conducted univariable meta-regression analyses to examine four a priori hypothesized moderators: pathogen class (Gram-positive, Gram-negative, or mixed), overall risk of bias (low/moderate vs high/critical), publication year (continuous), and time to positivity cutpoint (continuous, in hours). All meta-regression models were fitted using restricted maximum likelihood (REML) estimation, and moderator effects were assessed using the QM test statistic.

### Pathogen Class

Pathogen class did not significantly moderate the TTP-mortality association (QM = 3.97, df = 2, p = 0.137). Effect sizes were similar across Gram-positive (k = 12 studies), Gram-negative (k = 14 studies), and mixed pathogen populations (k = 7 studies). Compared to Gram-positive infections (reference category), the point estimates suggested numerically larger effects in Gram-negative (coefficient = 0.34 log-OR, 95% CI: -0.04 to 0.73, p = 0.068) and mixed infections (coefficient = 0.52 log-OR, 95% CI: -0.16 to 1.19, p = 0.126), but these differences were not statistically significant. Residual heterogeneity remained extremely high (I² = 98.3%), indicating that pathogen class explained only 0.3% of between-study variability. These findings are consistent with our stratified analysis demonstrating that TTP functions as a pathogen-agnostic prognostic marker.

### Risk of Bias

Overall risk of bias showed a trend toward moderation but did not reach statistical significance (QM = 2.74, df = 1, p = 0.098). Studies at high or critical risk of bias (k = 2) showed numerically smaller effect sizes compared to low or moderate risk studies (k = 31; coefficient = -0.40 log-OR, 95% CI: -0.88 to 0.08). However, the small number of high-risk studies limited statistical power to detect a moderator effect. Residual I² remained at 98.5%, representing only a 0.1% reduction from the baseline model. The lack of a significant risk of bias effect suggests that the TTP-mortality association is relatively robust to study quality, though the concentration of studies in the low-moderate risk category precluded definitive assessment.

### Publication Year

Publication year showed a borderline trend as a moderator (QM = 3.22, df = 1, p = 0.073) but did not reach conventional statistical significance. The positive coefficient (0.04 log-OR per year, 95% CI: -0.004 to 0.09) suggested that more recent studies tended to report slightly larger effect sizes, though the 95% confidence interval included zero. This trend may reflect improvements in TTP measurement technology, changes in patient populations, or increased attention to TTP as a prognostic marker in contemporary research. However, publication year explained minimal heterogeneity, with residual I² decreasing only from 98.6% to 98.0% (0.6% reduction). The non-significant finding indicates that the TTP-mortality association has remained relatively stable over the study period (1991-2024).

### Time to Positivity Cutpoint

In contrast to other moderators, TTP cutpoint emerged as a highly significant moderator of the association (QM = 11.01, df = 1, p < 0.001). Studies employing shorter TTP cutpoints reported significantly larger effect sizes than those using longer cutpoints (coefficient = -0.064 log-OR per hour, 95% CI: -0.10 to -0.03). This translates to an approximately 6.2% reduction in the pooled odds ratio for each additional hour of the TTP cutpoint threshold. For example, studies using an 8-hour cutpoint (vs 24-hour cutpoint) would be expected to show a pooled OR approximately 1.6-fold larger (16-hour difference × 6.2% per hour).

Examination of the bubble plot revealed this relationship visually: studies using cutpoints below 12 hours (k = 13) reported odds ratios ranging from approximately 2.5 to 8.0, whereas studies using cutpoints of 24 hours or greater (k = 5) reported more modest odds ratios between 1.0 and 2.5. This finding was robust after accounting for study precision, with larger studies showing the same trend as smaller studies.

Most importantly, TTP cutpoint was the only moderator that substantially reduced between-study heterogeneity, with residual I² decreasing from 98.6% to 71.3% (27.3% reduction, corresponding to a reduction in τ from 0.68 to 0.51). While 71.3% residual heterogeneity remained substantial, indicating that other unmeasured factors contribute to variability, TTP cutpoint explained approximately one-quarter of the observed heterogeneity—far exceeding the explanatory power of other examined moderators.

### Interpretation and Implications

The significant moderating effect of TTP cutpoint has important biological and methodological implications. Biologically, this finding suggests differential risk stratification depending on the time threshold used to dichotomize bacterial growth. Shorter cutpoints (e.g., 8-12 hours) may more specifically identify patients with extremely high bacterial inocula who are at highest risk for poor outcomes, whereas longer cutpoints (e.g., 24 hours) capture a broader, more heterogeneous population with variable bacterial loads and potentially diluted prognostic signal.

Methodologically, the finding highlights the importance of cutpoint selection in prognostic studies of TTP. Many included studies used data-driven cutpoint selection (e.g., via receiver operating characteristic curve analysis to identify optimal thresholds), which may have contributed to heterogeneity by selecting different cutpoints based on local population characteristics and event rates. This approach can optimize discrimination within individual studies but hinders comparability across studies. Future research should employ standardized cutpoints (e.g., 12 hours, the most commonly used threshold) to enhance comparability and facilitate evidence synthesis.

The lack of significant moderation by pathogen class reinforces our stratified analysis findings that TTP is a universal prognostic marker applicable across diverse bacterial pathogens. Similarly, the non-significant effect of risk of bias provides some reassurance regarding the robustness of findings across studies of varying methodological quality, though the limited number of high-risk studies precludes definitive conclusions.

The substantial residual heterogeneity (71.3%) after accounting for TTP cutpoint underscores that other unmeasured or inadequately captured factors contribute to between-study variability. Likely contributors include: (1) patient-level severity of illness (APACHE II, SOFA scores), which were inconsistently reported; (2) appropriateness and timing of empiric antibiotic therapy; (3) adequacy and timing of source control interventions; (4) underlying comorbidity burden; (5) blood culture system differences (BacT/ALERT, BACTEC) and incubation protocols; and (6) statistical adjustment approaches (unadjusted vs adjusted estimates with varying covariate sets). These unmeasured confounders likely explain why substantial heterogeneity persists even after accounting for the most influential observed moderator.

### Clinical and Research Recommendations

Based on these meta-regression findings, we recommend that clinicians interpret TTP cutpoints contextually, recognizing that very short TTP (<12 hours) may more specifically identify highest-risk patients requiring intensive monitoring and aggressive treatment. For researchers, we advocate for standardization of TTP measurement and reporting practices, including: (1) pre-specification of TTP cutpoints rather than data-driven selection; (2) reporting both dichotomized and continuous TTP analyses to facilitate dose-response meta-analyses; (3) standardizing TTP measurement protocols across blood culture systems; and (4) comprehensive reporting of key confounders (disease severity scores, antibiotic timing, source control details) to enable future individual patient data meta-analyses that can more definitively address residual heterogeneity.

---

## Summary

Meta-regression analyses revealed that TTP cutpoint significantly moderated the TTP-mortality association (p < 0.001), with shorter cutpoints associated with larger effect sizes and explaining 27% of between-study heterogeneity. Other examined moderators (pathogen class, risk of bias, publication year) did not significantly explain heterogeneity. The substantial residual heterogeneity (71%) suggests that unmeasured patient-level factors (disease severity, antibiotic timing, source control) and methodological differences contribute to between-study variability. These findings support TTP as a pathogen-agnostic prognostic marker while highlighting the need for standardized cutpoint selection and comprehensive confounder measurement in future studies.

---

**Word count:** ~1,100 words  
**Suitable for:** Results section of manuscript  
**Figures referenced:** MetaReg_Figure1-4  
**Table referenced:** Table 4

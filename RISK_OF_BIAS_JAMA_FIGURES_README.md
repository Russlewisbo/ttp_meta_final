# Risk of Bias Figures - JAMA Style

**Created:** March 7, 2026  
**Style:** JAMA (Journal of the American Medical Association)  
**Resolution:** 600 DPI (publication quality)  
**Studies:** n = 37

---

## Files Generated

### Figure_RiskOfBias_Overall_JAMA.png
**Dimensions:** 8" × 6"  
**Resolution:** 600 DPI  
**Size:** 203 KB  
**File Type:** PNG

**Description:**  
Bar chart showing the distribution of overall risk of bias across all 37 included studies. Each bar represents a risk category (Low, Moderate, High, Critical) with counts and percentages labeled above.

**Key Results:**
- Low risk: 10 studies (27.0%)
- Moderate risk: 25 studies (67.6%)
- High risk: 1 study (2.7%)
- Critical risk: 1 study (2.7%)

**Interpretation:** Two-thirds of studies have moderate overall risk, primarily driven by concerns in the Comparability domain.

---

### Figure_RiskOfBias_ByDomain_JAMA.png
**Dimensions:** 9" × 6.5"  
**Resolution:** 600 DPI  
**Size:** 330 KB  
**File Type:** PNG

**Description:**  
Stacked bar chart displaying risk of bias distribution across six assessment domains. Each bar shows the proportion of studies at each risk level within a domain.

**Key Results:**

| Domain | Low Risk | Moderate Risk | High Risk |
|--------|----------|---------------|-----------|
| Attrition | 31 (83.8%) | 6 (16.2%) | 0 (0%) |
| Statistical Analysis | 27 (73.0%) | 10 (27.0%) | 0 (0%) |
| Outcome Assessment | 20 (54.1%) | 17 (45.9%) | 0 (0%) |
| Prognostic Measurement | 18 (48.6%) | 16 (43.2%) | 3 (8.1%) |
| Selection | 14 (37.8%) | 22 (59.5%) | 1 (2.7%) |
| Comparability | 10 (27.0%) | 26 (70.3%) | 1 (2.7%) |

**Interpretation:** 
- **Best domain:** Attrition (83.8% low risk) - excellent follow-up completeness
- **Most problematic:** Comparability (70.3% moderate/high risk) - inadequate confounder adjustment

---

### Figure_RiskOfBias_Heatmap_JAMA.png
**Dimensions:** 9" × 13"  
**Resolution:** 600 DPI  
**Size:** 579 KB  
**File Type:** PNG

**Description:**  
Comprehensive heatmap showing risk of bias assessment for each study across all seven dimensions (six domains plus overall assessment). Color coding allows quick visual identification of patterns and problematic studies.

**Color Legend:**
- 🟢 Green: Low risk
- 🟠 Amber: Moderate risk
- 🔴 Red: High risk
- 🔴 Dark Red: Critical risk

**Interpretation:** Visual inspection reveals consistent moderate risk in Comparability across most studies, with heterogeneity in other domains.

---

## JAMA Style Specifications

### Typography
- **Font:** Arial (standard JAMA font family)
- **Title:** 13pt bold, dark gray (#2C3E50)
- **Subtitle:** 10-11pt regular, gray
- **Axis labels:** 10-11pt bold, dark gray
- **Data labels:** 9-10pt, varies by figure
- **Study names (heatmap):** 6.5pt for readability

### Color Scheme
**Professional muted palette:**
- **Primary text/borders:** Dark gray (#2C3E50)
- **Low risk:** Muted green (#5D9B59)
- **Moderate risk:** JAMA amber (#E69F00)
- **High risk:** Muted red (#CC503E)
- **Critical risk:** Dark red (#8B0000)

**Design principles:**
- Avoids overly bright colors
- Converts well to grayscale if needed
- Maintains visual hierarchy
- Professional appearance suitable for publication

### Layout
- **Background:** Pure white (#FFFFFF)
- **Gridlines:** Minimal, horizontal only where needed, subtle gray (#CCCCCC)
- **Borders:** Dark gray (#2C3E50), 0.5pt weight
- **Margins:** Adequate spacing for clarity
- **Legend position:** Top (domain chart), Right (heatmap), None (overall)

### Resolution & Format
- **DPI:** 600 (exceeds JAMA requirements)
  - JAMA minimum: 300 DPI for photos
  - JAMA preferred: 600 DPI for line art ✓
- **File format:** PNG with white background
- **Color mode:** RGB (converts cleanly to grayscale)
- **File size:** Optimized (203-579 KB)

---

## Usage Guidelines

### For Manuscript Submission

**Main Text:**
- Use **Figure_RiskOfBias_Overall_JAMA.png** as primary risk of bias figure
- Reference as "Figure X" in manuscript

**Supplementary Materials:**
- **Figure_RiskOfBias_ByDomain_JAMA.png** - detailed domain analysis
- **Figure_RiskOfBias_Heatmap_JAMA.png** - comprehensive study-level detail

### Suggested Figure Legends

#### Figure 1 (Overall)
> **Figure [X]. Risk of Bias Assessment for Included Studies.** Distribution of overall risk of bias among 37 studies included in the meta-analysis. Risk assessed using modified Newcastle-Ottawa Scale for cohort studies. Most studies (67.6%) had moderate overall risk, primarily due to inadequate adjustment for confounding variables in the Comparability domain. Numbers above bars indicate study counts with percentages in parentheses.

#### Figure 2 (By Domain)
> **Figure [X]. Risk of Bias by Assessment Domain.** Distribution of risk across six assessment domains for 37 included studies. Attrition showed the lowest risk (83.8% low risk), while Comparability was most problematic (70.3% moderate or high risk). Numbers within bars indicate study counts. Risk levels: green = low, amber = moderate, red = high.

#### Figure 3 (Heatmap)
> **Figure [X]. Study-Level Risk of Bias Assessment.** Comprehensive visualization of risk of bias across all studies and domains. Each row represents one study; each column represents an assessment dimension. The rightmost column shows overall risk of bias. Color coding: green = low risk, amber = moderate risk, red = high risk, dark red = critical risk. Assessment based on modified Newcastle-Ottawa Scale.

---

## Key Statistics Summary

### Overall Risk Distribution
```
Low:      10/37 (27.0%)
Moderate: 25/37 (67.6%)
High:      1/37 (2.7%)
Critical:  1/37 (2.7%)
```

### Domain Performance (% Low Risk)
```
1. Attrition:                83.8%  ← Best
2. Statistical Analysis:     73.0%
3. Outcome Assessment:       54.1%
4. Prognostic Measurement:   48.6%
5. Selection:                37.8%
6. Comparability:            27.0%  ← Most concerning
```

### Critical Issues Identified

**Comparability Domain (Most Problematic):**
- Only 10/37 studies (27%) had low risk
- Main issue: Inadequate confounder adjustment
- Common unmeasured confounders:
  - Disease severity (APACHE II, SOFA, Pitt scores)
  - Appropriateness of empiric antibiotics
  - Time to effective therapy
  - Source control adequacy
  - Comorbidity burden (Charlson index)

**Clinical Implication:**
- TTP may partially proxy for disease severity
- Observed associations could be confounded
- However, meta-regression showed ROB did NOT significantly modify effect estimates
- Findings appear robust despite methodological limitations

---

## Comparison with Previous Figures

### What Changed
| Aspect | Previous Version | JAMA Version |
|--------|-----------------|--------------|
| **Font** | System default | Arial |
| **Colors** | Bright saturated | Muted professional |
| **Gridlines** | Full grid | Minimal horizontal |
| **Text color** | Black | Dark gray (#2C3E50) |
| **Border weight** | Variable | Consistent 0.5pt |
| **Overall style** | Generic | JAMA publication standard |

### Consistency with Other JAMA Figures
✓ Matches Figure1_Forest_Mortality_JAMA.png style  
✓ Matches Figure2_Funnel_PublicationBias_JAMA.png style  
✓ Consistent typography and color scheme  
✓ Same resolution (600 DPI)  
✓ Same white background and margins  

---

## Clinical Interpretation

### Despite Moderate Risk, Findings Appear Robust

**Supporting Evidence:**
1. **Consistency:** TTP-mortality association consistent across studies with varying ROB levels
2. **Meta-regression:** Overall ROB did NOT significantly modify pooled estimates (95% CrI for ROB coefficient included zero)
3. **Sensitivity analysis:** Excluding high/critical risk studies (n=2) did not materially change pooled OR
4. **Bayesian regularization:** Robust estimation methods prevented undue influence of outliers
5. **Biological plausibility:** TTP reflects bacterial burden, a known prognostic factor

**Remaining Concerns:**
1. **Residual confounding:** Severity adjustment incomplete in most studies
2. **Observational design:** All included studies are cohort studies (no RCTs)
3. **TTP measurement:** Heterogeneous blood culture systems and protocols
4. **Publication bias:** Possible selective reporting (see funnel plot analysis)

**Overall Conclusion:**  
The moderate risk of bias is **acknowledged but does not invalidate the findings**. The TTP-mortality association appears genuine, though the magnitude may be partially confounded by disease severity. Future prospective studies with comprehensive severity adjustment would strengthen the evidence.

---

## Assessment Tool

**Newcastle-Ottawa Scale (Modified for Prognostic Factor Studies)**

**Domains Assessed:**
1. **Selection:** Representativeness of cohort, sample size justification
2. **Comparability:** Adjustment for confounders (severity, antibiotics, comorbidities)
3. **Outcome:** Objective assessment, adequate follow-up duration
4. **Statistical Analysis:** Appropriate methods, handling of missing data
5. **Attrition:** Loss to follow-up, reasons documented
6. **Prognostic Measurement:** TTP measured objectively, cutpoint pre-specified

**Risk Levels:**
- **Low:** Minimal bias concerns across all criteria
- **Moderate:** Some concerns but unlikely to seriously alter results
- **High:** Serious concerns that may substantially bias results
- **Critical:** Critical flaws that undermine confidence in findings

---

## Data Source

**File:** `TTP_Bias_Assessment_Included_Details.csv`  
**Studies:** 37 unique studies  
**Effect sizes:** 42 total (some studies contributed >1 effect)  
**Assessment date:** February 2026  
**Assessors:** [To be specified]  
**Inter-rater reliability:** [If applicable]

---

## Files for Download

All three JAMA-style figures are ready for:
- ✅ Journal manuscript submission
- ✅ Supplementary materials
- ✅ Conference presentations
- ✅ Grant applications
- ✅ Print publication

**Recommended citation format:**
> Lewis R. Time to Positivity as a Prognostic Marker in Bacteremia: A Bayesian Meta-Analysis. [Journal]. 2026. [In preparation]

---

## Version History

**Version 2.0** (March 7, 2026)
- Recreated in JAMA style for consistency with other project figures
- Corrected study count from "40" to accurate "37"
- Updated color palette to JAMA professional standards
- Applied Arial font family throughout
- Minimized gridlines for cleaner appearance
- 600 DPI publication-ready resolution

**Version 1.0** (February 19, 2026)
- Initial risk of bias visualization
- Generic ggplot2 styling

---

**Last updated:** March 7, 2026  
**Software:** R 4.5.1, ggplot2 4.0.2  
**Generated by:** Russell Lewis  
**Contact:** For questions about bias assessment or figure modifications

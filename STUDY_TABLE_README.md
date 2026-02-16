# TTP Meta-Analysis: Study Descriptive Table

## Overview

This directory contains a comprehensive descriptive summary table of all studies included in the Time to Positivity (TTP) meta-analysis examining the association between blood culture TTP and clinical outcomes in bacteremia.

## Files Generated

### 1. **TTP_Study_Descriptive_Table.csv**
- Raw CSV format with original variable names
- Suitable for further data manipulation in R/Python
- **Rows:** 54 studies
- **Columns:** 9 variables

### 2. **TTP_Study_Descriptive_Table_Formatted.csv**
- Publication-ready CSV with formatted column headers
- Human-readable column names
- Ideal for importing into Word/LaTeX tables

### 3. **TTP_Study_Descriptive_Table.html**
- Fully formatted HTML table with:
  - Color-coded risk of bias ratings (green = low, yellow = moderate, orange = high, red = critical)
  - Sortable columns
  - Professional formatting
  - Can be opened in any web browser

## Table Columns

| Column | Description |
|--------|-------------|
| **Author (Year)** | First author surname and publication year |
| **Country** | Country where study was conducted |
| **Study Design** | Study design type (retrospective cohort, prospective cohort, case-control, meta-analysis) |
| **N** | Total sample size |
| **Pathogen Class** | Gram classification (Gram-positive, Gram-negative, Mixed, Other) |
| **Specific Pathogen** | Organism(s) included (e.g., *S. aureus*, *E. coli*, *K. pneumoniae*) |
| **Main Outcome(s)** | Primary outcomes reported (Mortality, Persistent bacteremia, Clinical failure) |
| **TTP Cutoff** | Time to positivity cutpoint used (in hours) or "Continuous" if TTP was analyzed as continuous variable |
| **Risk of Bias** | Overall risk of bias assessment (low, moderate, high, critical) based on QUIPS tool |

## Summary Statistics

### Study Characteristics
- **Total studies:** 54
- **Total participants:** Variable (range reported in individual studies)
- **Study period:** 1991-2024 (enrollment dates)
- **Countries represented:** 18 countries across 5 continents

### Study Designs
- Retrospective cohort: 38 studies (70.4%)
- Prospective cohort: 13 studies (24.1%)
- Population-based cohort: 2 studies (3.7%)
- Meta-analysis: 1 study (1.9%)

### Pathogen Distribution
- Gram-positive BSI: 26 studies (48.1%)
  - *S. aureus* (most common)
  - *S. pneumoniae*
  - *S. pyogenes*
  - Coagulase-negative staphylococci
- Gram-negative BSI: 14 studies (25.9%)
  - *E. coli*
  - *K. pneumoniae*
  - *P. aeruginosa*
  - Other Enterobacteriaceae
- Mixed pathogen studies: 14 studies (25.9%)

### Outcomes Assessed
- **Mortality only:** 41 studies (75.9%)
  - 28-day mortality
  - 30-day mortality
  - In-hospital mortality
- **Mortality + Persistent bacteremia:** 5 studies (9.3%)
- **Persistent bacteremia only:** 4 studies (7.4%)
- **Other outcomes:** 4 studies (7.4%)
  - Clinical failure
  - ICU length of stay
  - Bacteremia classification

### TTP Cutoff Distribution
Common cutoffs used:
- **12 hours:** Most common
- **24 hours:** Frequently used
- **8 hours, 14 hours, 16 hours:** Less common
- **Continuous TTP:** Some studies analyzed TTP as continuous variable (per hour increase)

### Risk of Bias Assessment
- **Low risk:** 14 studies (25.9%)
- **Moderate risk:** 37 studies (68.5%)
- **High risk:** 2 studies (3.7%)
- **Critical risk:** 1 study (1.9%)

#### Domain-Specific Risk of Bias Notes:
- **Best domain:** Attrition (low risk in 84.4% of studies)
- **Most concerning domain:** Comparability (inadequate adjustment for confounders in 77.8% of studies)
- Common unmeasured confounders:
  - Disease severity scores (APACHE, SOFA)
  - Appropriateness of empiric therapy
  - Source control adequacy
  - Comorbidity burden

## Usage Examples

### In R:
```r
library(tidyverse)

# Load the table
studies <- read_csv("TTP_Study_Descriptive_Table_Formatted.csv")

# Filter by pathogen class
gram_pos_studies <- studies %>%
  filter(`Pathogen Class` == "Gram-positive")

# Count studies by country
studies %>%
  count(Country, sort = TRUE)
```

### In Python/Pandas:
```python
import pandas as pd

# Load the table
studies = pd.read_csv("TTP_Study_Descriptive_Table_Formatted.csv")

# Filter by study design
retrospective = studies[studies['Study Design'] == 'Retrospective cohort']

# Summarize TTP cutoffs
studies['TTP Cutoff'].value_counts()
```

### For Publication:
- Open the HTML file in a web browser
- Print to PDF for supplementary materials
- Or import CSV into Word/LaTeX table generators

## Notes on Data Quality

### Completeness
- All 54 studies have complete information for:
  - Author, year, country, design
  - Pathogen class
  - Main outcomes
  - Risk of bias assessment

### Missing/Variable Data
- **Sample sizes (N):** Some studies report multiple subgroups
- **Specific pathogens:** Listed as reported in original publications
- **TTP cutoffs:** Studies using continuous TTP marked as "Continuous"

### Exclusions
- 13 studies were excluded from the original 57 screened because they reported non-PICO outcomes or insufficient data
- Studies marked as `[NON-PICO]` in the database were excluded from this table

## Citation

When using this table, please cite:
> Lewis R. Time to Positivity in Bacteremia: A Bayesian Meta-Analysis. [In preparation]. 2026.

## Version Information

- **Table created:** February 16, 2026
- **Data source:** `TTP_MetaAnalysis_Extraction_Complete.xlsx`
- **Analysis software:** R 4.5.1
- **Packages used:** tidyverse, readxl, knitr, kableExtra, gt

## Contact

For questions about this table or the underlying data, please contact Russell Lewis.

---

**Last updated:** February 16, 2026

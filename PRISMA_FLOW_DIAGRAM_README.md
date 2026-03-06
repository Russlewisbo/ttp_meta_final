# PRISMA Flow Diagram - Study Selection

**Created:** March 6, 2026  
**Type:** Study selection flow diagram following PRISMA guidelines  
**Resolution:** 2400 × 3000 pixels (600 DPI at 4"×5")

---

## Files Generated

### 1. PRISMA_Flow_Diagram_Final.png
- **Format:** PNG
- **Resolution:** 2400 × 3000 pixels
- **Use:** Manuscript submission, online supplementary materials
- **Quality:** High resolution, suitable for publication

### 2. PRISMA_Flow_Diagram_Final.pdf
- **Format:** PDF (vector graphics)
- **Dimensions:** 8" × 10"
- **Use:** Print publication, high-quality reproduction
- **Quality:** Scalable vector format, no resolution loss

---

## Study Selection Summary

### Studies Included in Meta-Analysis

| Outcome | Studies (k) | Notes |
|---------|-------------|-------|
| **Mortality** | 33 | Primary outcome |
| **Persistent Bacteremia** | 9 | Secondary outcome |
| **Total unique studies** | 54 | Some studies reported multiple outcomes |
| **Total effect sizes** | 42 | Sum across all outcomes |

### PRISMA Flow Stages

The diagram shows the standard PRISMA flow through four stages:

1. **Identification**
   - Records identified through database searching (PubMed, Embase, Web of Science)
   - Additional records from reference lists and citations
   - Numbers for initial search not specified in available documentation

2. **Screening**
   - Duplicates removed
   - Title and abstract screening performed
   - Records excluded if not relevant to TTP and clinical outcomes

3. **Eligibility**
   - Full-text articles assessed for eligibility
   - Exclusion criteria applied:
     - Insufficient TTP data
     - No relevant outcomes (mortality or treatment failure)
     - Duplicate populations
     - Wrong study design

4. **Included**
   - **54 unique studies** included in qualitative synthesis
   - **33 studies** with mortality data in meta-analysis
   - **9 studies** with persistent bacteremia data in meta-analysis
   - Total of **42 effect sizes** across all outcomes

---

## Design Specifications

### Color Scheme (PRISMA Standard)

- **Identification stage:** Light blue (#E8F4F8)
- **Screening stage:** Light orange (#FFF4E6)
- **Eligibility stage:** Light green (#F0F8E8)
- **Included stage:** Green (#C8E6C8 to #E8F4E8)
- **Exclusions:** Light red (#FFE6E6)

### Typography

- **Font:** Arial
- **Box labels:** 11pt
- **Stage headers:** 12pt bold
- **Emphasis:** Bold for key numbers

### Layout

- **Direction:** Top-to-bottom flow
- **Box style:** Rounded rectangles with colored fills
- **Arrows:** Solid for inclusion flow, dashed for exclusions
- **Grouping:** Dashed boxes around each PRISMA stage

---

## Usage Guidelines

### For Manuscript Submission

1. **Main text:** Reference as "Figure S1" or "Supplementary Figure 1"
2. **Caption example:**
   > Figure S1. PRISMA flow diagram showing study selection process. Studies were identified through systematic database searching and reference list screening. After title/abstract screening and full-text review, 54 unique studies were included, providing 33 effect sizes for mortality analysis and 9 for persistent bacteremia analysis.

3. **File to submit:** Use `PRISMA_Flow_Diagram_Final.pdf` for journal submission (vector format preferred)

### For Presentations

- Use `PRISMA_Flow_Diagram_Final.png` for PowerPoint/Keynote
- High resolution ensures clarity even when enlarged
- Can crop or resize as needed

---

## Notes for Updating

### Missing Information

The following details should be added when available:

1. **Initial search results:**
   - Number of records identified through database searching
   - Number of additional records from other sources
   - Number after duplicate removal

2. **Screening numbers:**
   - Total records screened at title/abstract stage
   - Number excluded at screening

3. **Eligibility numbers:**
   - Total full-text articles assessed
   - Specific counts for each exclusion reason

### How to Update

If you obtain the missing numbers, you can update the diagram by:

1. Opening the R script used to generate it
2. Modifying the node labels with actual counts
3. Re-running the code to generate new PNG and PDF files

**R code location:** The diagram was generated using R with the `DiagrammeR`, `DiagrammeRsvg`, and `rsvg` packages.

---

## PRISMA Compliance

This flow diagram follows the **PRISMA 2020 Statement** guidelines:

- ✅ Shows all four stages: Identification, Screening, Eligibility, Included
- ✅ Indicates exclusions at each stage with reasons
- ✅ Provides final study counts for quantitative synthesis
- ✅ Uses standard PRISMA layout and terminology
- ⚠️ Some counts marked as "not specified" pending retrieval from study records

**Reference:**  
Page MJ, McKenzie JE, Bossuyt PM, et al. The PRISMA 2020 statement: an updated guideline for reporting systematic reviews. BMJ 2021;372:n71. doi: 10.1136/bmj.n71

---

## Study Characteristics

The 54 included studies span:

- **Publication years:** 2006-2025
- **Study designs:** Primarily retrospective and prospective cohorts
- **Pathogens:** Both Gram-positive and Gram-negative bacteria
- **Outcomes:** Mortality, persistent bacteremia, treatment failure
- **Countries:** 12+ countries represented
- **Settings:** Hospital-based bloodstream infection studies

**For detailed study characteristics, see:**
- TTP_Study_Descriptive_Table.csv
- TTP_Study_Characteristics_JAMA.pdf

---

**Last updated:** March 6, 2026  
**Generated by:** Russell Lewis  
**Software:** R 4.5.1, DiagrammeR, DiagrammeRsvg, rsvg

# HTML Summary Tables for Word Documents
## TTP Meta-Analysis Results Tables

**Created:** February 19, 2026  
**Format:** HTML tables ready for Microsoft Word  
**Purpose:** Summary of meta-analysis results in editable table format

---

## Files Created

### Table 1: Overall Mortality Meta-Analysis
**Filename:** `Table1_Mortality_Summary.html`  
**Content:** Complete summary statistics for mortality endpoint
- 33 effect sizes from 30 unique studies
- Bayesian pooled OR: 2.23 (95% CrI: 1.68–3.01)
- Frequentist validation
- Heterogeneity measures
- Publication bias assessment

### Table 2: Pathogen-Stratified Analysis
**Filename:** `Table2_Pathogen_Summary.html`  
**Content:** Side-by-side comparison of Gram-positive vs Gram-negative
- Gram-positive: OR 1.72 (k=13 studies)
- Gram-negative: OR 2.80 (k=14 studies)
- Statistical comparison showing no significant difference
- Conclusion: TTP is pathogen-agnostic marker

### Table 3: Persistent Bacteremia Meta-Analysis
**Filename:** `Table3_PersistentBacteremia_Summary.html`  
**Content:** Summary for persistent bacteremia/microbiological clearance
- 7 effect sizes from 6 unique studies
- Bayesian pooled OR: 1.95 (95% CrI: 0.53–6.24)
- Note about extreme outliers and high heterogeneity
- Interpretation guidance

---

## How to Use These Tables in Microsoft Word

### Method 1: Direct Paste (Recommended)

1. **Open the HTML file** in a web browser (Chrome, Firefox, Safari, Edge)
2. **Select the entire table** (click and drag, or Ctrl+A/Cmd+A)
3. **Copy** (Ctrl+C / Cmd+C)
4. **Open Microsoft Word**
5. **Paste** (Ctrl+V / Cmd+V)
6. The table will appear fully formatted with:
   - Header row (dark gray background, white text)
   - Alternating row colors (striped pattern)
   - Proper alignment
   - All formatting preserved

### Method 2: Paste Special

1. Follow steps 1-4 above
2. In Word, use **Paste Special** (Ctrl+Alt+V / Cmd+Option+V)
3. Select **HTML Format** or **Formatted Text (RTF)**
4. Click OK
5. Table appears with full formatting

### Method 3: Insert HTML Directly

1. In Word, go to **Insert → Object → Text from File**
2. Change file type filter to "All Files"
3. Select the `.html` file
4. Word will import the table with formatting

---

## Table Features

### Styling Applied

**Header Row:**
- Bold white text on dark gray background (#2C3E50)
- Consistent with JAMA style

**Alternating Rows:**
- White and light gray (#F0F0F0) striped pattern
- Improves readability

**Special Highlighting:**
- Section dividers (empty rows) with gray background
- Important notes highlighted in pale red (#FFE5E5) for persistent bacteremia table
- Comparison section in Table 2 has darker gray background

**Typography:**
- Font size: 12pt
- Clean, professional appearance
- Proper alignment (left for labels, right for values)

---

## Editing in Word

Once pasted, you can:

### Modify Content
- Click any cell to edit text
- Add or remove rows
- Update values

### Change Formatting
- Right-click → Table Properties
- Modify colors, borders, shading
- Adjust column widths

### Convert to Word Table Style
- Click table → Design tab
- Apply Word's built-in table styles if desired
- Or keep the HTML formatting

### Copy to PowerPoint
- Select table in Word
- Copy and paste into PowerPoint
- Formatting will be preserved

---

## Table Content Details

### Table 1: Mortality (Overall)

| Section | Contents |
|---------|----------|
| **Sample Size** | Studies (k), effect sizes, unique studies |
| **Bayesian Results** | Pooled OR with 95% CrI, posterior probabilities |
| **Frequentist Validation** | REML pooled OR with 95% CI, p-value |
| **Heterogeneity** | I² statistic, between-study SD (τ) |
| **Publication Bias** | Egger's test, trim-and-fill adjusted estimate |

**Key Result:** OR 2.23 with 100% posterior probability > 1

---

### Table 2: Pathogen-Stratified

| Section | Contents |
|---------|----------|
| **Sample Size** | Studies for each pathogen class |
| **Bayesian Results** | Pooled OR for Gram-positive and Gram-negative separately |
| **Frequentist Validation** | REML estimates for both groups |
| **Heterogeneity** | I² and τ for each group |
| **Comparison** | Statistical test of difference between groups |

**Key Result:** No significant difference (P(GP > GN) = 5.8%)

---

### Table 3: Persistent Bacteremia

| Section | Contents |
|---------|----------|
| **Sample Size** | Studies and effect sizes |
| **Bayesian Results** | Pooled OR with wide credible interval |
| **Frequentist Results** | Very wide confidence interval due to outliers |
| **Heterogeneity** | Extremely high (I² = 99.4%, τ = 2.74) |
| **Important Notes** | Warning about extreme outliers, interpretation guidance |

**Key Result:** OR 1.95 but with high uncertainty (P(OR > 1) = 85.3%)

---

## Formatting Notes

### If Formatting Is Lost

If paste doesn't preserve formatting:

1. **Use "Keep Source Formatting"** option when pasting
2. Or paste into a blank document first, then copy from there
3. Or use **Insert → Object → Text from File** method

### If Colors Don't Appear

- Ensure Word is not in "Print Layout" mode with "Show background colors"
- Check View → Web Layout (colors should appear)
- Or manually apply shading: Table Tools → Design → Shading

### If Table Is Too Wide

- Right-click table → AutoFit → AutoFit to Contents
- Or manually drag column borders
- Or set fixed column widths in Table Properties

---

## Customization Tips

### Change Color Scheme

To match your institution's colors:

1. Open HTML file in text editor
2. Find color codes (e.g., `#2C3E50`, `#F0F0F0`)
3. Replace with your colors
4. Save and re-open in browser
5. Copy to Word

### Add More Rows

In Word after pasting:
1. Click in last row
2. Press Tab to create new row
3. Type content
4. Apply formatting manually if needed

### Merge with Other Tables

- Copy multiple tables to create multi-panel table
- Use "Paste as Nested Table" if available
- Or place tables side-by-side using Word's table layout tools

---

## Table Captions for Manuscript

### Suggested Captions

**Table 1:**
> Table 1. Summary of Bayesian and Frequentist Meta-Analysis Results for Mortality Outcome. Shorter time to positivity (TTP) was associated with increased mortality (pooled OR 2.23, 95% credible interval 1.68–3.01) with 100% posterior probability. Substantial heterogeneity was observed (I² = 98.6%). Publication bias was detected (Egger's p < 0.001), but trim-and-fill analysis still indicated a positive association (OR 1.70). CrI, credible interval; OR, odds ratio; REML, restricted maximum likelihood.

**Table 2:**
> Table 2. Pathogen-Stratified Meta-Analysis of Mortality by Gram Stain. Both Gram-positive (OR 1.72) and Gram-negative (OR 2.80) infections showed positive associations between shorter TTP and mortality, with no statistically significant difference between groups (P(Gram-positive > Gram-negative) = 5.8%). This indicates TTP functions as a pathogen-agnostic prognostic marker. GP, Gram-positive; GN, Gram-negative.

**Table 3:**
> Table 3. Meta-Analysis of Persistent Bacteremia Outcome. Shorter TTP showed a positive but uncertain association with persistent bacteremia (OR 1.95, 95% CrI 0.53–6.24, P(OR > 1) = 85.3%). Extreme heterogeneity (I² = 99.4%) was driven by sparse-cell outliers (Melling2019). Bayesian estimate is more robust than the frequentist estimate in the presence of such outliers.

---

## Technical Details

### HTML Structure

Tables are created with:
- Bootstrap styling classes for professional appearance
- Inline CSS for colors and formatting
- Responsive design (adapts to container width)
- Accessibility features (proper header markup)

### Browser Compatibility

Tested in:
- ✅ Google Chrome (recommended)
- ✅ Mozilla Firefox
- ✅ Safari (macOS)
- ✅ Microsoft Edge

### Word Compatibility

Tested in:
- ✅ Microsoft Word 2016 or later (Windows)
- ✅ Microsoft Word 2016 or later (Mac)
- ✅ Microsoft 365 / Office 365
- ⚠️ Word 2013: May require "Keep Source Formatting" option

---

## Troubleshooting

### Problem: Table Doesn't Paste

**Solution:**
- Try Method 3 (Insert → Text from File)
- Or paste into Excel first, then copy to Word
- Check Word isn't in "Protected View" mode

### Problem: Formatting Looks Different

**Solution:**
- Use "Keep Source Formatting" when paste dialog appears
- Check Display settings in Word (Show background colors)
- Re-apply table styles manually if needed

### Problem: Special Characters Display Incorrectly

**Solution:**
- Ensure Word is set to UTF-8 encoding
- Re-save HTML file with UTF-8 encoding if edited
- Replace special characters (–, ×, ≥) manually in Word if needed

---

## Alternative Formats

If you need different formats:

### Excel
- Open HTML file in Excel
- Tables import automatically
- Save as .xlsx

### LaTeX
- Use `pandoc` to convert HTML to LaTeX table
- Or manually recreate using `booktabs` package

### CSV
- Open in Excel
- Save As → CSV
- Loses formatting but preserves data

---

## Location

**Files saved in:** `/Users/russelllewis/Desktop/ttp_meta_final/`

**Files created:**
1. `Table1_Mortality_Summary.html`
2. `Table2_Pathogen_Summary.html`
3. `Table3_PersistentBacteremia_Summary.html`

---

**Last updated:** February 19, 2026

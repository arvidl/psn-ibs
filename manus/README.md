# Manuscript: Patient Similarity Networks for IBS

This folder contains the LaTeX manuscript for submission to **Diagnostics** (MDPI).

## Files

- `psn_ibs_manuscript.tex` - Main LaTeX document
- `references.bib` - BibTeX bibliography
- `figs/` - Figures generated from the Jupyter notebook

## MDPI Template Setup

The manuscript uses the MDPI LaTeX template. To compile:

### 1. Download MDPI Template

Download the official MDPI LaTeX template from:
https://www.mdpi.com/authors/latex

Or directly:
```bash
# Create Definitions folder
mkdir -p Definitions

# Download template (you may need to download manually from MDPI website)
# The template includes: mdpi.cls, mdpi.bst, and other necessary files
```

### 2. Required Files in `Definitions/` folder

After downloading, place these files in the `Definitions/` folder:
- `mdpi.cls` - MDPI document class
- `mdpi.bst` - Bibliography style (optional, for BibTeX)

### 3. Generate Figures

Run the Jupyter notebook to generate figures:
```bash
cd ../notebooks
jupyter lab patient_similarity_networks_ibs_brain_morphometry_cognition.ipynb
```

Execute the notebook through Section 8 (Figure Export) to generate:
- `figs/fig1_communities.png`
- `figs/fig2_features.png`
- `figs/fig3_robustness.png`
- `figs/fig4_summary.png`
- `figs/fig_S1_community_features.png`

### 4. Compile LaTeX

```bash
# Using pdflatex and bibtex
pdflatex psn_ibs_manuscript
bibtex psn_ibs_manuscript
pdflatex psn_ibs_manuscript
pdflatex psn_ibs_manuscript

# Or using latexmk
latexmk -pdf psn_ibs_manuscript.tex
```

## Submission Checklist

- [ ] All figures generated and in `figs/` folder
- [ ] MDPI template files in `Definitions/` folder
- [ ] Bibliography entries complete
- [ ] Author ORCID updated
- [ ] Abstract within 200 words
- [ ] Keywords appropriate for Diagnostics
- [ ] Manuscript compiles without errors

## Journal Information

- **Journal**: Diagnostics
- **Publisher**: MDPI
- **Impact Factor**: 3.0 (2023)
- **Article Type**: Article
- **Special Issue**: (if applicable)

















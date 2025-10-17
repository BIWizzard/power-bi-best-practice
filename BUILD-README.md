# Building the Complete Guide

## Prerequisites

Choose one of these tools for PDF generation:

### Option 1: Pandoc (Recommended)
```bash
# Install Pandoc
brew install pandoc basictex  # macOS
# or download from: https://pandoc.org/installing.html
```

### Option 2: MkDocs with PDF Plugin
```bash
pip install mkdocs mkdocs-material mkdocs-with-pdf
```

## Generate PDF

### Using Pandoc
```bash
pandoc "00 - Introduction & Guide Overview.md" \
  "01 - Data Architecture & Semantic Modeling"/*.md \
  "02 - Performance Optimization & Query Design"/*.md \
  "03 - DAX Development Best Practices"/*.md \
  "04 - Report Design & User Experience"/*.md \
  "05 - Development Workflow & Version Control"/*.md \
  "06 - Governance Security & Deployment"/*.md \
  "07 - Continuous Learning & Community Resources"/*.md \
  --toc \
  --toc-depth=2 \
  --number-sections \
  --pdf-engine=xelatex \
  -V geometry:margin=1in \
  -V linkcolor:blue \
  -V urlcolor:blue \
  -o "AbsoluteCare_PowerBI_Best_Practices_Guide.pdf"
```

### Using MkDocs
1. Create `mkdocs.yml` configuration (see mkdocs.org for details)
2. Run: `mkdocs build`
3. PDF will be in `site/` directory

## Generate Static Website

### Using MkDocs
```bash
mkdocs serve  # Preview locally at http://127.0.0.1:8000
mkdocs build  # Generate static site in site/ directory
mkdocs gh-deploy  # Deploy to GitHub Pages
```

## Tips

- Preview markdown files in Obsidian or any markdown editor
- Use relative links between topics for better navigation
- Images in `_assets/images/` will be embedded in PDF
- Code blocks will be syntax-highlighted in PDF output

# {{PROJECT_NAME}}

{{PROJECT_NAME}} — brief description of the project or analysis.

## Getting Started

This template requires the TCDSB Quarto extensions and visual identity. After cloning, run:

```bash
# Install custom output formats
quarto add tcdsb/tcdsb-report-format
quarto add tcdsb/tcdsb-slide-format

# Install the TCDSB visual identity (colours, fonts, logos)
quarto use brand tcdsb/visual-identity
```

> These commands install into `_extensions/` and `_brand/` respectively. Neither directory is committed to the project repo.

## Project Structure

```
_example_pdf.qmd          # Example report (Typst PDF via tcdsb-report-format)
_example_presentation.qmd # Example slides (revealjs via tcdsb-slide-format)
R/
  00_Setup.R              # Shared setup: libraries, TCDSB theme
data/                     # Raw and processed data
output/                   # Rendered documents
```

## Rendering

```bash
quarto render _example_pdf.qmd
quarto render _example_presentation.qmd
```

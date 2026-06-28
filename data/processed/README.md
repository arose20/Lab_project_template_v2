# Processed Data

This directory contains analysis-ready, canonical datasets used for all downstream analysis.

It represents the "single source of truth" for modelling, visualisation, and interpretation.

## Key properties
- Stable and versioned
- Derived from raw data via reproducible pipelines
- Designed for repeated downstream use
- Modality-specific but harmonised within modality

## Examples
- Raw counts matrices (standardised format, e.g. AnnData/Seurat)
- Log-normalised expression matrices
- Integrated / batch-corrected datasets (if applicable)
- Final annotated datasets

## Rules
- Must be reproducible from raw data
- Should not contain experimental or competing transformations
- Changes only when pipeline logic changes
- Used as default input for analysis scripts

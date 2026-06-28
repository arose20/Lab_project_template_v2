# Source Code (`src/`)

This directory contains all core reusable scientific logic for the project.

It is the computational “brain” of the repository.

---

## Purpose

`src/` implements all domain-specific analysis logic, including:

- preprocessing
- QC
- statistical analysis
- modelling
- plotting utilities
- modality-specific pipelines (scRNA, spatial, metagenomics)

---

## Structure

Code should be organised by functional domain, not by execution order:

```text
src/
├── scrna/
├── spatial/
├── metagenomics/
├── preprocessing/
├── qc/
├── modelling/
├── plotting/
└── utils/
```

---

## Key Principles

- Code in `src/` must be **importable as a package**
- No execution logic should live here
- Must not directly read CLI arguments or run pipelines
- Must be reusable across scripts, workflows, and notebooks

---

## Rules

- Do NOT include hardcoded file paths
- Do NOT write outputs directly (handled by interfaces/workflows)
- Do NOT duplicate logic found elsewhere
- Must remain independent of execution environment
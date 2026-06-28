# Interfaces (`interfaces/`)

This directory contains all user-facing entry points to the project.

It is the “interaction layer” between users and core logic.

---

## Purpose

Interfaces provide controlled access to:

- workflows
- analysis functions
- pipeline execution
- exports

---

## Types of Interfaces

### CLI Interfaces
Command-line entry points for running analyses.

### Python Interfaces
Reusable APIs for programmatic use.

### External Integration
Wrappers for tools like:
- Nextflow
- Snakemake
- HPC submission systems

---

## Structure

```text
interfaces/
├── cli/
├── python/
└── pipelines/
```

---

## Rules

- Must call functions from `src/` or `workflows/`
- Must NOT contain scientific logic
- Must remain stable and user-facing
- Should act as thin wrappers only
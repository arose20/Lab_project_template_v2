# Scripts (`scripts/`)

This directory contains lightweight executable wrappers for project functionality.

---

## Purpose

Scripts provide simple entry points for common tasks such as:

- running QC
- launching analyses
- exporting results
- triggering workflows

---

## Structure

```text
scripts/
├── scrna/
├── spatial/
├── metagenomics/
├── qc/
└── utils/
```

---

## Key Principle

> Scripts are glue, not logic

---

## Rules

- Must call `src/` or `workflows/`
- Must NOT implement analysis logic
- Must remain minimal and replaceable
- Should be safe to delete without losing functionality

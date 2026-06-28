# Workflows (`workflows/`)

This directory defines computational pipelines and execution logic.

---

## Purpose

Workflows define:
- task orchestration
- data flow
- execution order
- compute distribution

---

## Key Principle

> Workflows define execution, not analysis logic

All scientific computation must live in `src/`.

---

## Structure

```text
workflows/
├── nextflow/
├── snakemake/
├── modules/
└── configs/
```

---

## Rules

- Must call `src/` functions
- Must be fully configurable via `config/`
- Must remain modular and composable
- Must not contain embedded scientific logic

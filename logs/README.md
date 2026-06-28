# Logs (`logs/`)

This directory contains execution logs from all system components of the project.

Logs are used for debugging, auditing, and reproducibility tracking.

---

## Purpose

Logs capture **execution behaviour**, not scientific results.

They are essential for:

- debugging failures
- tracking pipeline execution
- monitoring compute environments
- auditing data movement

---

## Structure

```text
logs/
├── pipelines/
├── notebooks/
├── scripts/
├── sync/
└── system/
```

---

## Categories

### pipelines/
Workflow execution logs (Nextflow, Snakemake, etc.)

### notebooks/
Execution logs from nbconvert, papermill, or compute notebook runs

### scripts/
Logs from CLI or analysis scripts

### sync/
Logs from rsync and data transfers between storage systems

### system/
SLURM logs, environment logs, runtime diagnostics

---

## Key Principle

> Logs describe how computation happened, not what was produced

---

## Rules

- Logs are operational artifacts
- Logs may be regenerated unless required for audit
- Do NOT store scientific outputs in logs/
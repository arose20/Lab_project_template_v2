# Notebooks (`notebooks/`)

This directory contains exploratory and narrative analyses.

---

## Purpose

Notebooks are used for:

- exploratory data analysis (EDA)
- figure development
- hypothesis generation
- interactive debugging
- communication of results

---

## Key Principle

> Notebooks are for exploration, not production pipelines

---

## Rules

- Must NOT contain production logic
- Must call functions from `src/`
- Must be reproducible end-to-end
- Should be convertible to reports when needed (e.g. nbconvert)

---

## Execution

When run on compute nodes:
- outputs and logs are captured in `logs/notebooks/`
- rendered outputs should be stored in `results/reports/`

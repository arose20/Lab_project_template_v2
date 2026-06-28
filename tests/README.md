# Tests (`tests/`)

This directory contains automated validation for the project.

---

## Purpose

Ensures correctness and reproducibility of:

- core functions in `src/`
- workflows
- configuration parsing
- data integrity

---

## Structure

```text
tests/
├── unit/
├── integration/
├── data_validation/
└── pipelines/
```

---

## Key Principle

> If it can break reproducibility, it should be testable

---

## Rules

- Tests must be deterministic
- Tests should run quickly where possible
- Large dataset tests must be explicitly marked
- Must not depend on external compute environments unless required
# br-parse-viz-demo

## Overview

This repository demonstrates:
- GitHub branch protection & code review workflow
- Automated CI via GitHub Actions

---

## Branching Workflow

- Protected `main` branch
- Features developed in branches like `feature/parser-service`
- Pull Requests enforced, reviewed, and CI-checked before merging

---

## GitHub Actions CI

- Workflow at `.github/workflows/ci.yml` runs on every PR
- Uses `pytest` for automated testing

---

## How to Run

```bash
pip install -r requirements.txt
uvicorn main:app --reload
pytest

# MLOps Roadmap — Oct 2026 → Apr 2027

**Goal:** land an MLOps job by April 2027.
**Certification:** AWS Certified Machine Learning Engineer – Associate (MLA-C02, standard version expected early 2027).
**Time budget:** ~2h per weekday + weekends (~12h/week, ~300h total).

---

## Overview

| Month | Period | Focus | Key tools |
|---|---|---|---|
| 1 | Oct | PyTorch refresh, project structure, experiment tracking, data versioning | PyTorch, uv, ruff, pytest, MLflow, DVC |
| 2 | Nov | CI/CD for ML, model serving, GPU containers | GitHub Actions, FastAPI, Docker |
| 3 | Dec | Kubernetes on my own cluster (desktop + Pi 4) | k3s, kubectl, Helm |
| 4 | Jan | Monitoring, data drift, orchestration — **start applying** | Prometheus, Grafana, Evidently, Prefect |
| 5 | Feb | AWS / SageMaker, move part of the capstone to the cloud | AWS, SageMaker |
| 6 | Mar–Apr | Exam + portfolio polish | — |

---

## Month 1 — Foundations (Oct 6 → Nov 1)

| Week | Focus | Done when… |
|---|---|---|
| 1 (Oct 6–11) | Tensors, autograd, `nn.Module`, `Dataset`/`DataLoader`, training loop on GPU | A small image classifier trains on the RTX 3080 with a hand-written loop, reproducible with fixed seeds |
| 2 (Oct 12–18) | `src` layout, `pyproject.toml`, uv, ruff, pytest, pre-commit, config files | Week 1 code is a clean installable package with tests; training runs from one command |
| 3 (Oct 19–25) | MLflow: runs, params, metrics, artifacts, model registry; self-hosted with Docker Compose + MinIO | Several runs compared in the MLflow UI; best model registered |
| 4 (Oct 26–Nov 1) | DVC: data tracking, remotes, `dvc.yaml` pipelines, `dvc repro` | Full pipeline (data → train → evaluate) reproducible with one command |

**Month 1 milestone:** capstone topic chosen, with a one-page project brief.

---

## Capstone criteria

- Data that changes over time (so drift monitoring makes sense in month 4)
- Trainable on an RTX 3080 (10 GB VRAM)
- Servable through an API
- Not a toy dataset (no MNIST-style projects)

Topic: _TBD by Nov 1_

---

## Progress tracking

- **LEARNING_LOG.md**: 3 lines after each session (learned / blocked / next).
- **Weekly check-in** (Sunday): share the week's log, short quiz, adjust next week.
- **Project instructions**: update the "Current status" line at each milestone.

---

## Status

- [ ] Month 1 — Foundations
- [ ] Month 2 — CI/CD & serving
- [ ] Month 3 — Kubernetes
- [ ] Month 4 — Monitoring & orchestration
- [ ] Month 5 — AWS / SageMaker
- [ ] Month 6 — Exam & portfolio

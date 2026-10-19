# David — AI Evaluation Engineer

I build **reproducible, CI-enforced evaluation systems for LLM/RAG products**:
the quality / safety / cost / latency / governance signal on one side, adversarial
(red-team) robustness on the other — wired into a release gate instead of a
dashboard nobody reads.

## Flagship work

### [eval-quality-gate](https://github.com/David899b/eval-quality-gate) — 5-dimension release gate

[![quality](https://github.com/David899b/eval-quality-gate/actions/workflows/quality.yml/badge.svg)](https://github.com/David899b/eval-quality-gate/actions/workflows/quality.yml)

Gates a model on **quality, safety, cost, latency and governance**, and emits a
decision (`GO` / `REVIEW` / `NO_GO`) with a confidence band computed from three
scenarios (pessimistic / base / optimistic). Demo decision: **REVIEW**.

### [eval-redteam-suite](https://github.com/David899b/eval-redteam-suite) — OWASP-aligned red-team gate

[![quality](https://github.com/David899b/eval-redteam-suite/actions/workflows/quality.yml/badge.svg)](https://github.com/David899b/eval-redteam-suite/actions/workflows/quality.yml)

Runs an attack corpus against a target and computes **Attack Success Rate (ASR)**
per OWASP LLM Top 10 category, blocking on vulnerability. Demo decision:
**NO_GO** against a deliberately vulnerable target.

### [eval-pipeline](https://github.com/David899b/eval-pipeline) — one CI pipeline, both gates

[![pipeline](https://github.com/David899b/eval-pipeline/actions/workflows/pipeline.yml/badge.svg)](https://github.com/David899b/eval-pipeline/actions/workflows/pipeline.yml)

Chains both gates and produces a single roll-up plus an evidence artifact, so one
pipeline backs a release decision end-to-end.

## What I care about

- Every number anchors to a **measurable baseline**.
- Always **three scenarios** — never a single point estimate.
- Reproducible and **first-run-ready**: clone, run, get the same result.
- Fewer dependencies, more determinism.

## Skills

Python · pytest · CI/CD (GitHub Actions) · LLM evaluation harnesses · red-teaming
/ OWASP LLM Top 10 · RAG metrics · cost & latency budgets · model cards &
governance.

## Contact

- GitHub: [@David899b](https://github.com/David899b)

# Human Agency Lab — AI Credit Evaluation

An interactive workshop simulator for **Human Agency by Design**. Participants design *where and how* a human intervenes in an AI-driven personal-loan workflow, then run a realistic portfolio and observe the trade-offs.

## What it does

- **Scenario → Configure → Run → Optimize → Reflect** (the full workshop arc).
- Five intervention points (data collection, evaluation, decision, execution, communication) plus five system sliders (confidence threshold, risk tolerance, review cost, error severity, reversibility).
- A **seeded Monte Carlo simulation** of 240 synthetic applicants — realistic score / DTI / segment distributions, model miscalibration and bias against thin-file & irregular-income borrowers, data errors, imperfect human review, appeals (adverse-action / ECOA-style), and expected financial outcome (interest margin vs loss-given-default).
- Five illustrative named cases, including one the model rejects at **94% confidence but is wrong** — the pedagogical core: confidence-based routing alone never catches it.
- A multi-dimensional **Human Agency Score** (oversight, contestability, learning) shown against performance (accuracy, speed, cost) and a fairness gap — deliberately *not* a single number.

Results are reproducible (fixed seed), so any given design always yields the same numbers — ideal for comparing team variants.

## Run locally

Just open `index.html` in a browser. No build, no dependencies.

## Deploy on Render

This repo ships a `render.yaml` blueprint (static site). In Render:

1. **New → Blueprint**, connect this repository → it auto-detects `render.yaml`.
   *(Or: New → Static Site, publish directory `.`, no build command.)*
2. Deploy. The site is served from `index.html`.

Fictional, simplified system for educational use.

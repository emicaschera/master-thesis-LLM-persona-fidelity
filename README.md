# Measuring the Fidelity of Language Models (LLMs)
## Persona-Profile-Based Evaluation in the Political Domain — Master’s Thesis

**Author:** Emilio Caschera  
**Degree:** M.Sc. Computer Engineering (Artificial Intelligence & Machine Learning) — Roma Tre University  
**Academic Year:** 2024/2025

📄 **Download the thesis (PDF):** `thesis.pdf`

---

## Abstract 
This thesis investigates whether Large Language Models (LLMs) can approximate **real human survey responses** in politically salient domains when impersonating **survey-grounded personas** (multi-attribute profiles built from socio-demographic and attitudinal variables).  
The evaluation is performed on the Italian subsample of **European Social Survey (ESS) Round 11 (2023–2024)**, comparing human responses against multiple LLMs under controlled replication and prompting constraints.

---

## What this work is about (in 30 seconds)
- Builds **multi-attribute personas** derived from real survey respondents (decision-tree segmentation).
- Queries LLMs to **impersonate** each persona with **replicated runs** under fixed seeds.
- Compares synthetic vs real answers in:
  - **observable space** (transparent 0–100 composite score)
  - **latent space** (PCA estimated on real data, then model projections)
- Measures: **bias**, **variance compression**, **rank-order fidelity**, and **correlation structure**.

---

## Key contributions / highlights
- **Persona evaluation grid**: 28 multi-attribute personas (with minimum support per persona).
- **Symmetric comparability design**: 30 human respondents per persona vs **30 LLM replications** per persona.
- **Transparent scoring**: composite 0–100 score built from three ESS items.
- **Latent-space assessment**: PCA fitted on real profiles only; LLMs projected into “human space”.
- Findings show systematic deviations (e.g., **location bias** and **variance compression**) while preserving much of the **profile ordering**.

---

## Methods & tools (high-level)
- **Prompt engineering** with strict JSON output constraints.
- Replicated sampling with **fixed seeds** to study stability vs human variability.
- Statistical comparison across profiles:
  - mean error / MAE
  - dispersion ratios
  - Pearson correlation (ordering fidelity)
  - PCA-based latent alignment

---

## Keywords 
**LLM Evaluation, Prompt Engineering, Persona Modeling, Synthetic Data, Survey Simulation, Bias & Calibration, Reproducibility, PCA, Experimental Design, Python, JSON-constrained generation, Social Data / ESS**

---

## Repository contents
- `thesis.pdf` — full thesis document
- `README.md` — this page



## How to cite
If you reference this work, please cite the thesis:

```bibtex
@mastersthesis{caschera2025llm_persona_fidelity,
  title  = {Measuring the Fidelity of Language Models: A Persona-Profile-Based Evaluation in the Political Domain},
  author = {Caschera, Emilio},
  school = {Roma Tre University},
  year   = {2025},
  type   = {Master's Thesis}
}

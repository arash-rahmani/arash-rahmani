# Arash Rahmani — Computational Biologist
> 10% Noise. 90% Signal.
M.Sc. Bioinformatics · Julius-Maximilians-Universität Würzburg<br>
Python · Reproducible pipelines · From genome to mind<br>
Open to opportunities in Germany & beyond

---

## What I build

I write Python pipelines that turn complex biological and behavioral data into reproducible, auditable results — without the chaos that usually comes with academic code.

The same architectural philosophy applies across both domains: config-driven, schema-validated, pytest-tested, modular. The data changes. The rigor doesn't.

---

## Pipelines

### [obf-psychiatric-pipeline](https://github.com/arash-rahmani/obf-psychiatric-pipeline) · 2026

Classification of psychiatric conditions from wrist-worn motor activity.
OBF-Psychiatric dataset · 76 participants · 3-class and binary framing

- Participant-level GroupKFold CV · bootstrap 95% CIs · 112 pytest tests
- Binary control-vs-patient: macro-F1 **0.849** (95% CI 0.761–0.920) — combined features, XGBoost
- 3-class control/depression/schizophrenia: macro-F1 **0.753** (95% CI 0.645–0.841) — combined features, logistic regression
- Custom temporal feature extraction from raw actigraphy: interdaily stability, intradaily variability, L5/M10, cosinor parameters, Cole-Kripke sleep metrics
- Logistic regression · XGBoost · SHAP feature attribution
- Config-driven · schema-validated · modular

**Scientific finding:** Temporal and circadian features alone (F1 0.699) outperform distributional features alone (F1 0.595) on 3-class psychiatric classification — meaning rhythmic structure carries disorder-specific information that activity volume statistics do not. Combined features push 3-class discrimination from 0.595 to **0.753**, a +0.158 improvement over the distributional baseline. The engineering choice of *which features to compute* moved the needle, not model complexity. SHAP attribution on the combined classifier recovers a textbook chronobiological finding: cosinor acrophase (delayed activity peak) is the dominant feature distinguishing depression, while schizophrenia shows the opposite acrophase direction — distinct circadian signatures across disorders. Paper in preparation.

`Python` `scikit-learn` `XGBoost` `SHAP` `pandas` `NumPy` `pytest`

---

### [rnaseq-python-pipeline](https://github.com/arash-rahmani/rnaseq-python-pipeline) · 2025

Reproducible RNA-seq differential expression and pathway enrichment in Python.
Validated on *Fagus sylvatica* transcriptomics (carbon harvesting, CO₂ conditions)

- End-to-end: raw counts → QC → differential expression → GSEA pathway enrichment
- Config-driven · pytest-tested · modular src-layout package
- PyDESeq2 for differential expression · gseapy for enrichment

`Python` `PyDESeq2` `gseapy` `pandas` `NumPy` `matplotlib` `pytest`

---

## The bridge

These two pipelines are not coincidental. Genomic data sits inside tight evolutionary corridors — conditions separate cleanly, signals are crisp. Behavioral data is biology unconstrained — humans on medication, in wards, having lives. The engineering philosophy transfers. The interpretation changes.

What started as distributional motor classification — strong on binary, weak on 3-class — became a methodological question: *can the right features recover disorder-specific signal?* They can. Temporal and circadian structure separates depression from schizophrenia in a way activity volume statistics cannot. Engineering effort pays in discovery.

---

## Stack

```
Languages:   Python · R · Bash
ML:          scikit-learn · XGBoost · SHAP
Bio:         PyDESeq2 · gseapy · HISAT2 · StringTie · DESeq2 · clusterProfiler
Signal:      cosinor analysis · Cole-Kripke sleep scoring · circadian rhythm features
Practices:   pytest · Git · YAML config-driven design · schema validation · bootstrap CI
```

---

## Connect

[LinkedIn](https://linkedin.com/in/arash-rahmani-544684242) · Würzburg, Germany

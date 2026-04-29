# Arash Rahmani — Computational Biologist

> 10% Noise. 90% Signal.

M.Sc. Bioinformatics · Julius-Maximilians-Universität Würzburg
Python · Reproducible pipelines · From genome to mind
Open to opportunities in Germany & beyond

---

## What I build

I write Python pipelines that turn complex biological and behavioral data into reproducible, auditable results — without the chaos that usually comes with academic code.

The same architectural philosophy applies across both domains: config-driven, schema-validated, pytest-tested, modular. The data changes. The rigor doesn't.

---

## Pipelines

### [obf-psychiatric-pipeline](https://github.com/arash-rahmani/obf-psychiatric-pipeline) · 2026
Classification of psychiatric conditions from wrist-worn motor activity.

OBF-Psychiatric dataset · 77 participants · 3-class and binary framing

- Participant-level GroupKFold cross-validation · bootstrap 95% CIs
- Binary control-vs-patient: macro-F1 **0.80** (95% CI 0.70–0.88)
- 3-class control/depression/schizophrenia: macro-F1 0.60 (95% CI 0.48–0.71)
- Logistic regression · XGBoost · SHAP feature attribution
- Config-driven · schema-validated · 17+ pytest tests

**Finding:** distributional motor features reliably separate inpatients from healthy controls but cannot distinguish depression from schizophrenia — a shared low-activity signature that reflects inpatient status and medication effects more than disorder-specific behavior. Temporal/circadian features are the next experiment.

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

The next iteration computes temporal features from raw actigraphy — interdaily stability, intradaily variability, cosinor amplitude — to test whether rhythmic structure can disambiguate what distributional summaries cannot.

---

## Stack

```
Languages:   Python · R · Bash
ML:          scikit-learn · XGBoost · SHAP
Bio:         PyDESeq2 · gseapy · HISAT2 · StringTie · DESeq2 · clusterProfiler
Practices:   pytest · Git · YAML config-driven design · schema validation · bootstrap CI
```

---

## Connect

[LinkedIn](https://linkedin.com/in/arash-rahmani-544684242) · Würzburg, Germany

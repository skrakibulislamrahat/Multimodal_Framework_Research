# Explainable Multimodal Diabetic-Retinopathy Research Prototype

This repository contains an experimental deep-learning workflow that combines **retinal fundus images** with a tabular metadata branch for diabetic-retinopathy modeling and explainability.

## What the project implements

- APTOS 2019 retinal fundus images
- EfficientNetB0 image feature extraction
- a small MLP/tabular branch
- late feature fusion for classification
- Grad-CAM-style image interpretation
- SHAP-based analysis for the tabular branch
- cross-validation and Messidor-2 external-validation notebooks tracked separately in this repository

## Critical methodological scope

The clinical/tabular variables in the original framework notebook are **synthetically generated for architecture prototyping**; they are not observed patient metadata. That distinction is essential. Results from this branch must therefore be interpreted as a proof-of-concept for multimodal fusion mechanics, **not evidence that real clinical metadata improves DR prediction**.

See [`LIMITATIONS.md`](LIMITATIONS.md) before using or citing this project.

## Repository contents

```text
.
├── DR_Multimodal_Framework_Colab_Notebook.ipynb   # original fusion prototype
├── DR_Multimodal_Cross_Validation_FIXED.ipynb     # cross-validation workflow
├── DR_Multimodal_External_Validation.ipynb        # external-validation workflow
├── LIMITATIONS.md
├── requirements.txt
└── README.md
```

## Research question

The useful question represented by this repository is architectural: **how can retinal-image features and structured covariates be fused and interpreted in a single DR modeling pipeline?**

A clinically valid answer would require real, patient-linked covariates collected under an appropriate study protocol, leakage-safe data splits, external validation, and calibration analysis.

## Reproducibility

The notebooks were developed in Google Colab and use local Google Drive paths. Raw APTOS/Messidor image data and model checkpoints are not distributed in Git. Users should update data paths and record package versions, hardware, random seeds, and dataset releases when reproducing experiments.

## Research status

This is a **research prototype**, not a clinical multimodal validation study. The repository is retained because the fusion architecture, interpretability workflow, and evaluation scaffolding are useful research artifacts when that limitation is stated explicitly.

## Responsible use

This code is for research and education. It is not a clinical diagnostic system and should not be used for patient-care decisions.

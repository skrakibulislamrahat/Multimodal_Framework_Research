# An Explainable Multimodal Fusion Framework for Diabetic Retinopathy Detection

This repository contains the full Colab notebook, model results, and Grad-CAM visualizations for our study on early detection of diabetic retinopathy (DR) using a multimodal deep learning framework.

## 🔍 Objective

To develop an explainable AI system that combines retinal fundus images and simulated clinical features (e.g., HbA1c, blood pressure, duration of diabetes) for accurate DR classification and real-world deployment in rural and resource-constrained settings.

## 📁 Contents

- `DR_Multimodal_Fusion_Final.ipynb` — the complete Colab notebook with:
  - EfficientNetB0 + MLP fusion model
  - Image preprocessing
  - Clinical metadata simulation
  - Grad-CAM visualization
  - Evaluation metrics (accuracy, F1-score, AUC)
- `/figures/` — Grad-CAM outputs for Moderate and Proliferative DR
- `results/` — optional CSV or logs of predictions (if any)

## 🧠 Model Overview

- Visual input: APTOS 2019 fundus images (n=3,662)
- Tabular input: 5 simulated features per patient
- Model: Dual-branch CNN + dense fusion
- Metrics:
  - **Val Accuracy**: 81.3%
  - **F1-Score**: 0.80 (weighted)
  - **AUC**: 0.936

## 📊 Explainability

- Grad-CAM used to visualize model attention on fundus images
- SHAP used to interpret clinical feature importance

## 🚀 Deployment Scope

The model is designed for:
- Clinical decision support
- Teleophthalmology
- Mobile and rural screening programs

## 📝 Citation

If you use this work, please cite:


# Multimodal_Framework_Research

This repository contains the full implementation for the research paper:

**"Explainable Deep Learning Framework for Early Detection of Diabetic Retinopathy in Retinal Imaging: A Scalable Approach for Clinical and Rural Deployment"**

### 👥 Authors:
- Md Reazul Islam Karim  
- Yasin Arafat  
- Prof. Makul Mahajan  
- Prof. Dr. Murtaza Hussain *(Research Advisor)*  
- SK Rakib Ul Islam Rahat

---

## 🧠 Overview

This project presents a multimodal and explainable deep learning framework that combines:

- **High-resolution fundus images** (APTOS 2019)
- **Simulated clinical metadata** (age, HbA1c, BP, BMI, etc.)
- **EfficientNetB0** for image feature extraction
- **MLP** for metadata fusion
- **Grad-CAM** and **SHAP** for interpretability

The model is evaluated through:
- ✅ 5-fold cross-validation (APTOS)
- ✅ External validation (Messidor-2)
- ✅ Grad-CAM & SHAP visualizations

---

## 🔍 Contents

```bash
📁 DR_Multimodal_Cross_Validation_FIXED.ipynb   # 5-fold APTOS training & eval
📁 DR_Multimodal_External_Validation.ipynb      # Messidor-2 validation
📁 DR_Multimodal_Framework_Colab_Notebook.ipynb # Unified pipeline version
📄 README.md

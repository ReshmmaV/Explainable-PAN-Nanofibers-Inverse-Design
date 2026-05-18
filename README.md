# Explainable PAN Nanofibers Inverse Design

![Python](https://img.shields.io/badge/Python-3.10-blue)
![PyTorch](https://img.shields.io/badge/PyTorch-DeepLearning-red)
![XAI](https://img.shields.io/badge/Explainable-AI-green)
![Springer](https://img.shields.io/badge/Publication-Springer-success)

## Uncertainty-Aware Inversion and Explainable Electron Microscope Image-Based Defect Analysis Framework for Electrospun Polyacrylonitrile Nanofibers

This repository presents a comprehensive AI-driven framework for inverse design and defect analysis of electrospun Polyacrylonitrile (PAN) nanofibers using uncertainty-aware machine learning, Bayesian Optimization, Explainable AI (XAI), and electron microscope image analysis.

The framework combines:
- Process-Structure-Property-Quality (PSPQ) modeling
- Uncertainty-aware inverse parameter optimization
- Bayesian Optimization for target fiber diameter prediction
- SHAP-based interpretability
- SEM image-based defect analysis
- ConvNeXt-Tiny feature extraction
- Explainable AI for defect localization

---

# Overview

Electrospun Polyacrylonitrile (PAN) nanofibers are widely used in tissue engineering due to their extracellular matrix-like structure. However, achieving structurally uniform nanofibers with desired fiber diameters remains challenging because electrospinning depends on multiple interacting factors including:

- Polymer solution rheology
- Electrostatics
- Environmental thermodynamics
- Process parameters

Traditional optimization relies heavily on trial-and-error experimentation.

This work proposes a unified AI-driven framework to:
1. Learn PSPQ relationships for PAN electrospinning
2. Perform uncertainty-aware inverse design for desired fiber diameters
3. Analyze SEM images for defect identification
4. Provide explainable predictions using XAI techniques

---

# Abstract

Electrospun polyacrylonitrile (PAN) is widely used in tissue engineering as it mimics the extracellular matrix. Consistent production of electrospun PAN nanofibers with structural uniformity and desired fiber diameter remains challenging, as electrospinning depends on various factors including rheology of the polymer solution, environmental thermodynamics, and electrostatics, mandating extensive trial-and-error approaches.

The present study develops a combined framework to understand the Process-Structure-Property-Quality (PSPQ) relationship of PAN and determine electrospinning parameters capable of producing structurally uniform and fixed-diameter PAN nanofibers.

A Random Forest regressor trained on PAN electrospinning parameters from the Cogni-e-Spin 1.0 dataset achieved:
- RMSE: 0.16
- R² Score: 0.6

Bootstrap resampling was incorporated for uncertainty estimation, followed by Bayesian Optimization to determine electrospinning parameters for desired fiber diameters (e.g., 150 nm to 250 nm).

SHapley Additive exPlanations (SHAP) analysis confirmed that solution concentration significantly influences fiber diameter.

Additionally, a hybrid computer vision pipeline was developed for defective electrospun fiber analysis using SEM images from the Figshare PAN nanofiber dataset. The framework extracted features using a pre-trained ConvNeXt-Tiny model followed by Random Forest classification.

The proposed defect analysis framework achieved:
- Accuracy: 97.16%
- AUROC: 0.997
- AUPRC: 0.997
- MCC: 0.994
- Cohen’s Kappa: 0.943

Explainable AI achieved a test fidelity of 81.7%.

The proposed framework enables intelligent determination of electrospinning process parameters for desired nanofiber synthesis while simultaneously identifying post-synthesis defects. The framework can also be extended to other electrospun polymers.

---

# Publication

This work is accepted/published in Springer Proceedings in Physics.

### Citation

Vijayakumar, R., Venkatesan, N.

**Uncertainty Aware Inversion and an Explainable Electron Microscope Image-based Defect Analysis Framework for Electrospun Polyacrylonitrile Nanofibers**

Proceedings of the International Conference on Recent Advancement in Physical Sciences (ICAPS-2026).

Springer Proceedings in Physics.

Publisher:
Springer Nature Singapore Pte Ltd.

---

# Keywords

- Biomaterials
- Polyacrylonitrile
- Electrospinning
- Inverse Design
- Uncertainty Quantification
- Bayesian Optimization
- ConvNeXt-Tiny
- Explainable AI
- PSPQ Modeling
- SEM Image Analysis
- Nanofiber Defect Detection

---

# Technical Contributions

## Inverse Design Framework
- PSPQ relationship modeling
- Random Forest surrogate modeling
- Bootstrap uncertainty estimation
- Bayesian Optimization
- Target fiber diameter prediction
- SHAP-based parameter interpretability

## Defect Analysis Framework
- SEM image-based defect classification
- ConvNeXt-Tiny feature extraction
- Random Forest classification
- Explainable AI analysis
- Hybrid deep learning pipeline

---

# Model Performance

## Inverse Design Model

| Metric | Value |
|---|---|
| RMSE | 0.16 |
| R² Score | 0.6 |

---

## Defect Analysis Model

| Metric | Value |
|---|---|
| Accuracy | 97.16% |
| AUROC | 0.997 |
| AUPRC | 0.997 |
| MCC | 0.994 |
| Cohen’s Kappa | 0.943 |
| XAI Fidelity | 81.7% |

---

# Repository Structure

```text
Explainable-PAN-Nanofibers-Inverse-Design/

│
├── Inverse_Design/
│   ├── Surrogate_Model.ipynb
│   ├── Bayesian_Optimization.ipynb
│   ├── SHAP_Analysis.ipynb
│   └── Uncertainty_Analysis.ipynb
│
├── Defect_Analysis/
│   ├── ConvNeXt_RF.ipynb
│   ├── XAI_Analysis.ipynb
│   └── Evaluation.ipynb
│
├── images/
├── results/
├── README.md
├── requirements.txt
└── LICENSE
```

---

# Datasets

## Electrospinning Dataset
- Cogni-e-Spin 1.0 dataset

## SEM Defect Dataset
- PAN Nanofiber SEM Dataset from Figshare

Note:
Datasets may be subject to licensing or research restrictions and are therefore not directly uploaded in this repository.

---

# Technologies Used

- Python
- PyTorch
- Scikit-learn
- ConvNeXt-Tiny
- Random Forest
- Bayesian Optimization
- SHAP
- Explainable AI (XAI)
- OpenCV
- NumPy
- Pandas
- Matplotlib

---

# Workflow

## Inverse Design Pipeline

1. Electrospinning parameter preprocessing
2. Surrogate model training
3. Uncertainty estimation using bootstrap resampling
4. Bayesian Optimization
5. SHAP explainability analysis
6. Target nanofiber diameter prediction

---

## Defect Analysis Pipeline

1. SEM image preprocessing
2. Feature extraction using ConvNeXt-Tiny
3. Random Forest classification
4. Defect prediction
5. Explainable AI visualization
6. Performance evaluation

---

# Results

The proposed framework successfully:
- Predicted optimal electrospinning parameters
- Generated target nanofiber diameter recommendations
- Identified nanofiber defects with high accuracy
- Provided interpretable AI explanations
- Reduced dependency on trial-and-error experimentation

---

# Applications

- Tissue Engineering
- Biomaterials Manufacturing
- Smart Nanomaterial Synthesis
- AI-assisted Electrospinning
- Automated SEM Analysis
- Materials Informatics
- Autonomous Materials Discovery

---

# Future Scope

- Real-time electrospinning optimization
- Reinforcement learning-assisted synthesis
- Autonomous nanomaterial manufacturing
- Multi-polymer electrospinning analysis
- Real-time SEM defect inspection systems
- Edge AI deployment for manufacturing environments

---

# Authors

- Reshmma Vijayakumar
- Nandakumar Venkatesan

---

# License

This repository is intended for academic and research purposes only.

---

# Acknowledgement

The authors acknowledge Springer Nature and the ICAPS-2026 conference for supporting the dissemination of this work.

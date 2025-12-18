# Ebserh Clinical Outcomes – Project Repository

This repository contains the code, notebooks, and files used in the project for predicting hospital outcomes at the Federal University of Pelotas University Hospital (HE-UFPel), including mortality, length of stay, and 30-day readmission.

> **Disclaimer:** The original codebase existed in a different directory structure. Therefore, **relative paths may not work out of the box** when running the notebooks in this organized version. This structure was created solely to improve **transparency, documentation, and partial reproducibility**, while preserving the logic and results of the original development.

---

## 📁 Repository Structure

The main folder is:

```
clinical-outcomes-code/
├── files/
└── notebooks/
```

### **1. `files/`**

Contains **all auxiliary artifacts** generated throughout the project, including:

* Extracted **JSON** files.
* **Preprocessed datasets**: `X_train`, `X_test`, etc.
* **Model output results**.
* **Selected feature lists** (e.g., Boruta outputs).
* CID lists used for **encoding**.
* Files with **strong correlations** (e.g., PHIK results).
* Other miscellaneous files relevant to the ML pipeline.

This directory serves as an archive for important intermediate artifacts and final results.

---

### **2. `notebooks/`**

Organized by the main stages of the machine learning pipeline.

#### **2.1. `ANALYSIS/`**

Complementary analysis notebooks, including:

* SHAP value interpretation.
* PCA and UMAP for dimensionality reduction.
* **PHIK** correlation analysis.
* **ROC curves**.

#### **2.2. `PREDICTION/`**

* Contains notebooks used for model training, validation, and evaluation.

#### **2.3. `PREPROCESSING/`**

* Contains notebooks used for preprocessing.

---

## 🎯 Project Objective

To develop machine learning models capable of predicting clinical outcomes using structured clinical and administrative data from HE-UFPel. These predictions can support medical teams and hospital management in risk monitoring, resource allocation, and decision-making.

---

## ⚠ Important Notes

* Notebook paths reflect their **original development environment**, so they **will not run directly** without path adjustments.
* Files are organized here to promote **transparency**, **clear navigation**, and a **structured view** of the ML workflow.
* All sensitive data has been removed or anonymized following institutional and ethical guidelines.

---
**🧩 Environment Setup**

A environment.yml file is available in the root directory of the project. It contains all dependencies required to correctly reproduce the environment used during development, including Python version, main libraries, and additional packages installed via pip.

To create the environment, run:

```
conda env create -f environment.yml
conda activate ebserh-clinical-outcomes
```

This ensures that all notebooks and scripts have access to the correct versions of the tools used in the project.
---

## Contact

If you have questions or suggestions regarding the codebase or repository organization, please open an issue or contact the project team.

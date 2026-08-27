# Heart Disease Prediction — Cross‑Hospital Stability Study
**Authors:** Hardik Varma, Aryan  
**Affiliation:** Pune, India  
**Target Journal:** IJCOPE (Deadline: Aug 31, 2026)
---
## 📌 Overview
This project investigates **how well different machine learning models generalise across hospital populations**. Unlike existing studies that train on combined data from multiple hospitals, we **train exclusively on Cleveland** and test on Hungary, Switzerland, and VA Long Beach **without retraining**.
**Key Question:** *Which model type stays most reliable when deployed at a different hospital?*
---
## 🧠 Models Used
- Logistic Regression
- Random Forest
- Support Vector Machine (SVM)
- K‑Nearest Neighbours (KNN)
- XGBoost
---
## 📊 Key Finding
| Model | F1 Spread (Max‑Min) |
| :--- | :--- |
| **SVM** | **0.050** (most stable) |
| Random Forest | 0.053 |
| KNN | 0.081 |
| XGBoost | 0.102 |
| Logistic Regression | 0.227 (least stable) |
**Conclusion:** SVM and Random Forest are robust across populations; Logistic Regression collapses on Switzerland (F1 drops to 0.559).
---
## 📁 Repository Structure
```text
├── data/                    # Cleveland, Hungary, Switzerland, VA datasets
├── results/                 # Metrics tables and stability charts
├── code/                    # Python scripts and notebooks
├── paper/                   # Journal templates and paper drafts
├── archive/                 # Prior drafts and reference files
├── requirements.txt         # Dependencies
└── README.md                # Project documentation

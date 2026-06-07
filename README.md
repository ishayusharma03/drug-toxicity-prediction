# 🧪 AI-Driven Drug Toxicity Prediction

> Predicting drug toxicity across 12 biological pathways using machine learning and molecular fingerprinting — with SHAP explainability.

---

## 📌 Overview

This project builds a machine learning pipeline to predict whether chemical compounds are toxic across 12 different biological pathways, using the **Tox21 dataset** (7,831 compounds). It combines cheminformatics (RDKit) with ensemble ML models and SHAP-based explainability to provide interpretable toxicity predictions.

---

## ✨ Features

- 🧬 **Molecular Feature Engineering** – Morgan fingerprints and molecular descriptors from SMILES strings via RDKit
- 🤖 **Multi-label Classification** – Predicts toxicity across 12 biological pathways simultaneously
- 📈 **Multiple ML Models** – Logistic Regression, Random Forest, Gradient Boosting, XGBoost
- 🔎 **SHAP Explainability** – Identifies key molecular substructures driving toxicity predictions
- 📊 **Comprehensive Evaluation** – ROC-AUC, confusion matrices, and per-pathway performance metrics

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python |
| Cheminformatics | RDKit |
| ML Models | Scikit-Learn, XGBoost |
| Explainability | SHAP |
| Data Processing | Pandas, NumPy |
| Dataset | Tox21 (7,831 compounds, 12 pathways) |

---

## 📊 Results

| Model | Avg. ROC-AUC |
|-------|-------------|
| Logistic Regression | — |
| Gradient Boosting | — |
| XGBoost | — |
| **Random Forest** | **0.838** ✅ Best |

> Random Forest delivered the strongest overall performance with an average ROC-AUC of **0.838** across all 12 toxicity pathways.

---

## 🚀 Getting Started

```bash
# Clone the repository
git clone https://github.com/ishayu-sharma/drug-toxicity-prediction.git
cd drug-toxicity-prediction

# Install dependencies
pip install -r requirements.txt

# Run the pipeline
python train.py
```

### Requirements
```
rdkit
scikit-learn
xgboost
shap
pandas
numpy
matplotlib
```

---

## 📁 Project Structure

```
drug-toxicity-prediction/
├── data/
│   └── tox21.csv               # Tox21 dataset
├── features/
│   └── fingerprints.py         # Morgan fingerprint generation
├── models/
│   ├── random_forest.py
│   ├── xgboost_model.py
│   └── logistic_regression.py
├── explainability/
│   └── shap_analysis.py        # SHAP feature importance
├── train.py                    # Main training script
├── evaluate.py                 # Evaluation & metrics
├── requirements.txt
└── README.md
```

---

## 🔬 Tox21 Pathways Covered

The model predicts toxicity for 12 biological assays including:
`NR-AR` · `NR-AR-LBD` · `NR-AhR` · `NR-Aromatase` · `NR-ER` · `NR-ER-LBD` · `NR-PPAR-gamma` · `SR-ARE` · `SR-ATAD5` · `SR-HSE` · `SR-MMP` · `SR-p53`

---

## 👤 Author

**Ishayu Sharma**  
[LinkedIn](https://linkedin.com/in/ishayu-sharma-567a252b2) · [Email](mailto:ishayusharma03@gmail.com)

# 🔄 Kaggle — Predict Customer Churn (Playground S6E3)

Kaggle competition solution for predicting customer churn in a telecom dataset.

---

## 📊 Approach

| Model | CV AUC |
|-------|--------|
| Baseline LightGBM | 0.91604 |
| Ensemble LGB + XGB + CatBoost | 0.91653 |
| + Tuned LightGBM (Optuna) | 0.91658 |
| **Optimized blend (final)** | **0.91665** |

## 🔍 Key EDA Findings

- **Contract type** is the strongest churn signal — month-to-month: 42.1% churn vs two-year: 1.0%
- **New customers** churn most — 49.4% in first 12 months
- **Fiber optic** has highest churn (41.5%) despite being the premium service
- **Higher monthly charges** correlate strongly with churn

## 🛠️ Tech Stack

- **LightGBM, XGBoost, CatBoost** — gradient boosting ensemble
- **Optuna** — Bayesian hyperparameter optimization
- **Scipy** — blend weight optimization
- **StratifiedKFold** — 5-fold cross-validation

## 📁 Structure

```
kaggle-churn-prediction/
├── data/          # Download from Kaggle (not included)
├── eda_baseline_ensemble.ipynb
└── README.md
```

## 📦 Dataset

[Kaggle — Playground Series S6E3](https://www.kaggle.com/competitions/playground-series-s6e3)

---

## 👤 Author

**Yulia Vovk** | 📍 Tokyo | [GitHub](https://github.com/yumilin92)

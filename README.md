# Explainable Anxiety & Depression Prediction

An explainable, uncertainty-aware ML framework for predicting anxiety and depression risk from demographic and psychological questionnaire data (PHQ-9, GAD-7, PSS, ISI), using optimized XGBoost, SHAP-based interpretability, and counterfactual reasoning.

## What's inside

- Separate XGBoost models for anxiety and depression, tuned with 5-fold CV
- Validation-based decision threshold selection and probability calibration
- SHAP global (summary/bar) and local (waterfall) explanations
- Counterfactual analysis: minimal feature changes that flip a prediction
- Subgroup/fairness evaluation across demographic groups

## Results (final test set)

| Target | Accuracy | F1 | ROC-AUC |
|---|---|---|---|
| Anxiety | 97.59% | 0.532 | 0.960 |
| Depression | 94.62% | 0.508 | 0.939 |

## Getting started

```bash
pip install -r requirements.txt
jupyter notebook anxiety_depression_prediction.ipynb
```

> Dataset not included — add your own data file and update the path at the top of the notebook.

## Disclaimer

This is a research/educational project for risk screening support — not a diagnostic tool. Not a substitute for professional clinical assessment.

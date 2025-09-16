# Week 6 — Iris Classifier (Tuned)

**Date:** 2025-09-15 23:47
**Dataset:** Iris (scikit-learn)

## Methods
- Pipeline: StandardScaler + estimator
- CV: StratifiedKFold (5-fold)
- Tuning:
  - KNN: n_neighbors, weights, p (GridSearchCV)
  - SVC (RBF): C, gamma (RandomizedSearchCV)

## Leaderboard (sorted by CV F1-macro)
| model           |   cv_f1_macro_mean |   cv_f1_macro_std |   test_acc |   test_f1_macro |   test_roc_auc_ovr |
|:----------------|-------------------:|------------------:|-----------:|----------------:|-------------------:|
| Best_KNN        |             0.9821 |            0.022  |     0.9737 |          0.9743 |             0.9938 |
| Baseline_LogReg |             0.9638 |            0.0528 |     0.9211 |          0.923  |             0.9959 |
| Best_SVC        |             0.9638 |            0.0528 |     0.9737 |          0.9743 |             0.9979 |

**Winner:** Best_KNN

## Artifacts
- Saved model: `/Users/vicev/models_week6/Best_KNN_iris.pkl`
- Leaderboard CSV: `/Users/vicev/models_week6/leaderboard_week6_iris.csv`

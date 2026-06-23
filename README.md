# 🩺 Diabetes Classification — Random Forest + GridSearchCV

![Python](https://img.shields.io/badge/Python-3.8+-blue?logo=python)
![scikit-learn](https://img.shields.io/badge/scikit--learn-1.0+-orange?logo=scikit-learn)
![Task](https://img.shields.io/badge/Task-Classification-green)
![Dataset](https://img.shields.io/badge/Dataset-Pima%20Indians%20Diabetes-lightgrey)

---

## 📌 Project Overview

Binary classification model to predict whether a patient has **diabetes** based on medical diagnostic measurements.

| Item | Detail |
|------|--------|
| **Dataset** | Pima Indians Diabetes Dataset (768 patients) |
| **Model** | Random Forest + GridSearchCV |
| **Metric** | Precision (minimize false positives in medical context) |
| **Target** | `Outcome` → 1 = Diabetes, 0 = Healthy |

---

## 🗂️ Project Structure

```
01_diabetes_classification/
├── main.ipynb        ← Full notebook: EDA → Train → Evaluate → Visualize
├── dataset_info.md   ← Download link + column descriptions
└── README.md         ← This file
```

---

## 🚀 How to Run

### Step 1 — Install dependencies
```bash
pip install pandas numpy scikit-learn matplotlib seaborn openpyxl
```

### Step 2 — Download dataset
👉 [Pima Indians Diabetes Dataset on Kaggle](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)

Place `diabetes.csv` **or** `diabetes.xlsx` in this folder.

### Step 3 — Open notebook
```bash
jupyter notebook main.ipynb
```
Then click **Kernel → Restart & Run All**

---

## ⚙️ ML Pipeline

```
diabetes.csv / diabetes.xlsx
        │
        ▼
Train / Test Split (80% / 20%)
        │
        ▼
StandardScaler
        │
        ▼
GridSearchCV × RandomForestClassifier
  ├── n_estimators    : [50, 100, 200, 500]
  ├── criterion       : [gini, entropy, log_loss]
  ├── max_depth       : [None, 2, 5]
  └── min_samples_split: [2, 5, 10]
        │
        ▼
Evaluate → Classification Report + Confusion Matrix + Feature Importance
```

---

## 📊 Results

| Class | Precision | Recall | F1-Score |
|-------|-----------|--------|----------|
| Healthy (0) | ~0.85 | ~0.90 | ~0.87 |
| Diabetes (1) | ~0.78 | ~0.68 | ~0.73 |

**Charts generated:**
- 📊 Class Distribution
- 🔥 Correlation Heatmap
- 🟦 Confusion Matrix
- 📈 Feature Importance

---

## 🔑 Key Concepts

- ✅ Binary classification with imbalanced classes
- ✅ Feature scaling with `StandardScaler`
- ✅ Hyperparameter tuning with `GridSearchCV` (6-fold CV)
- ✅ Precision-optimized model for medical use case
- ✅ Feature importance visualization

---

## 📦 Dependencies

```
pandas
numpy
scikit-learn
matplotlib
seaborn
openpyxl
```

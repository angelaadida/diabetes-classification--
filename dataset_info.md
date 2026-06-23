# 📊 Dataset Info — Pima Indians Diabetes Dataset

## 🔗 Download Link

👉 **Kaggle:** https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database

> **How to download:**
> 1. Go to the link above
> 2. Click the **Download** button (top right)
> 3. Save file as `diabetes.csv` or `diabetes.xlsx`
> 4. Place it in the same folder as `main.ipynb`

---

## 📋 Column Descriptions

| Column | Type | Description |
|--------|------|-------------|
| `Pregnancies` | int | Number of times pregnant |
| `Glucose` | int | Plasma glucose concentration (2-hour test) |
| `BloodPressure` | int | Diastolic blood pressure (mm Hg) |
| `SkinThickness` | int | Triceps skinfold thickness (mm) |
| `Insulin` | int | 2-Hour serum insulin (mu U/ml) |
| `BMI` | float | Body mass index (kg/m²) |
| `DiabetesPedigreeFunction` | float | Genetic likelihood score |
| `Age` | int | Age in years |
| `Outcome` | int | **Target** — 1 = Diabetes, 0 = Healthy |

- **Total rows:** 768 patients
- **Features:** 8 input features + 1 target
- **Class balance:** ~65% Healthy (0), ~35% Diabetes (1)

---

## ⚠️ Note on File Format

This notebook **automatically detects** your file format:
- ✅ `diabetes.csv` → works directly
- ✅ `diabetes.xlsx` → also works (no need to rename!)

Both formats are supported out of the box.

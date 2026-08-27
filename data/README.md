<< 'EOF'
# Data Description

## Source
**UCI Heart Disease Dataset**  
Available at: https://archive.ics.uci.edu/ml/datasets/heart+Disease

---

## Hospitals Included

| Hospital | Abbreviation | # Patients |
| :--- | :--- | :--- |
| Cleveland Clinic (USA) | Cleveland | 304 |
| Hungarian Institute of Cardiology (Hungary) | Hungary | 293 |
| University Hospital Zurich (Switzerland) | Switzerland | 123 |
| VA Long Beach (USA) | VA Long Beach | 200 |

**Total:** 920 patients

---

## Features Used (10 Common Features)

| Feature | Description |
| :--- | :--- |
| `age` | Age in years |
| `sex` | 0 = Female, 1 = Male |
| `cp` | Chest pain type (0-3) |
| `trestbps` | Resting blood pressure (mm Hg) |
| `chol` | Serum cholesterol (mg/dl) |
| `fbs` | Fasting blood sugar > 120 mg/dl (0/1) |
| `restecg` | Resting ECG results (0-2) |
| `thalch` | Maximum heart rate achieved |
| `exang` | Exercise-induced angina (0/1) |
| `oldpeak` | ST depression induced by exercise |

---

## Target Variable

- `num` = 0 → No disease
- `num` = 1 → Disease present
(Original was 0-4, binarized to 0/1)

---

## Files

| File | Description |
| :--- | :--- |
| `heart_disease_uci.csv` | Raw combined dataset |
| `cleveland_cleaned.csv` | Cleveland only, cleaned, 10 features |
| `hungary_cleaned.csv` | Hungary only, cleaned, 10 features |
| `switzerland_cleaned.csv` | Switzerland only, cleaned, 10 features |
| `va_long_beach_cleaned.csv` | VA Long Beach only, cleaned, 10 features |

---

## Preprocessing Notes

- Imputation: **Cleveland-only** median/mode used for all missing values
- Scaling: **Cleveland-only** StandardScaler used to transform all datasets
- **No data leakage** — test hospitals never used for imputation or scaling
EOF


\# Key Findings Summary — For Introduction \& Abstract



\## Dataset

\- \*\*Source:\*\* UCI Heart Disease dataset

\- \*\*Hospitals:\*\* Cleveland (304), Hungary (293), Switzerland (123), VA Long Beach (200)

\- \*\*Total:\*\* 920 patients

\- \*\*Features:\*\* 10 clinical features (age, sex, cp, trestbps, chol, fbs, restecg, thalch, exang, oldpeak)

\- \*\*Target:\*\* Binary (0 = no disease, 1 = disease present)



\## Experimental Design

\- \*\*Training:\*\* 80% of Cleveland only

\- \*\*Testing:\*\* 20% of Cleveland + 100% of Hungary, Switzerland, VA Long Beach

\- \*\*Models:\*\* Logistic Regression, Random Forest, SVM, KNN, XGBoost

\- \*\*Key Metric:\*\* F1 Score and Spread (Max-Min F1 across hospitals)



\## Key Results



\### F1 Spread (Lower = More Stable)

| Model | Spread |

| :--- | :--- |

| SVM | 0.050 |

| Random Forest | 0.053 |

| KNN | 0.081 |

| XGBoost | 0.102 |

| Logistic Regression | 0.227 |



\### Main Finding

\- \*\*SVM and Random Forest\*\* are most stable across hospitals (spread \~0.05)

\- \*\*Logistic Regression\*\* collapses on Switzerland (F1 drops from 0.764 to 0.559)

\- \*\*All models\*\* perform worse on Switzerland than other hospitals



\### Clinical Implication

\- Models trained on one hospital population \*\*do not generalize equally\*\* to other populations

\- Linear models (LR) are especially vulnerable to population shifts

\- Non-parametric/ensemble methods (SVM, RF) are more robust



\## Limitations (to mention in Introduction/Abstract)

\- Data collected 1983-1988 (\~40 years old)

\- Small sample size (only \~240 training patients)

\- Only 10 features used

\- \*\*Not clinically deployable\*\* — this is a methodological study


#  Task 4: Loan Default Prediction – Data Science Internship

##  Objective
Build a machine learning model to predict if a loan applicant is likely to default using financial data.  
This helps lenders reduce credit risk and avoid losses.

---

##  Dataset

- **Name**: German Credit Dataset  
- **Source**: [UCI Repository](https://archive.ics.uci.edu/ml/datasets/statlog+(german+credit+data))  
- **Rows**: 1000  
- **Features**: 20 categorical/numerical  
- **Target**: 0 = Fully Paid, 1 = Default

---

##  Workflow

### 1. Data Preprocessing
- Renamed columns, converted target values
- Encoded categorical columns using Label Encoding
- Scaled features using StandardScaler

### 2. Handling Imbalance
- Used SMOTE to upsample default class (30% → 50%)

### 3. Model Training
- LightGBM (best performance)
- Evaluated with F1-score, Precision, Recall, AUC-ROC

### 4. Evaluation
- AUC: ~0.80
- ROC Curve plotted
- Precision-Recall trade-off examined

---

##  Results

| Metric        | Score (LightGBM) |
|---------------|------------------|
| Precision     | ~0.77            |
| Recall        | ~0.78            |
| F1-Score      | ~0.77            |
| AUC-ROC       | ~0.80            |

---

##  Insights

- High credit amount and short history increase default risk
- SMOTE improved detection of minority class (defaults)
- Model useful for banks to flag risky applications

---

## Tools Used

- Python 3.12  
- pandas, scikit-learn, imbalanced-learn  
- lightgbm, matplotlib, seaborn

---


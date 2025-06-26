#  Task 1: Employee Attrition Prediction – Data Science Internship

##  Objective

Build a machine learning model to predict whether an employee is likely to leave a company based on HR analytics data. The model is also used to generate explainable insights that can help HR design retention strategies.

---

##  Dataset

- **Source**: IBM HR Analytics Employee Attrition & Performance
- **Link**: [Kaggle - IBM HR Analytics Dataset](https://www.kaggle.com/datasets/pavansubhasht/ibm-hr-analytics-attrition-dataset)
- **Records**: 1,470 employees
- **Target Variable**: `Attrition` (Yes/No)
- **Features**: Demographics, job satisfaction, income, travel, experience, etc.

---

## Steps Performed

### 1. Exploratory Data Analysis (EDA)
- Analyzed attrition rates and patterns
- Identified important features like `OverTime`, `MonthlyIncome`, `JobSatisfaction`
- Plotted visualizations to support insights

### 2. Data Preprocessing
- Removed uninformative columns (`EmployeeNumber`, `Over18`, etc.)
- Applied label encoding and one-hot encoding
- Train-test split (80/20) with stratification

### 3. Modeling
-  Random Forest Classifier (best results)
-  Logistic Regression (baseline)
- Evaluation metrics: Accuracy, Precision, Recall, F1 Score, Confusion Matrix

### 4. Explainability
- Used **SHAP (SHapley Additive Explanations)** to explain feature importance
- Identified top features driving attrition

---

##  Key Visualizations

- Countplot: Attrition distribution
- Boxplot: Monthly Income vs Attrition
- Confusion Matrix: Model performance
- SHAP Bar Plot: Feature importance

---

##  Key Insights

- Employees working overtime are more likely to leave
- Lower salary and satisfaction levels increase attrition
- Young/new employees need better engagement strategies
- Certain job roles (e.g., Sales Rep) have higher turnover

---

##  Tools Used

- Python 3.12
- Pandas, NumPy, Matplotlib, Seaborn
- scikit-learn (RandomForest, LogisticRegression)
- SHAP for explainability

---

##  Report & Submission

- Report: `Task1_Attrition_Report.pdf`
- Code, plots, and visuals included as supporting files
- Dataset
---

##  Final Notes

This project demonstrates a complete ML pipeline from data cleaning to modeling and interpretation, aligned with real-world HR analytics problems. The model helps HR teams identify at-risk employees and take proactive retention steps.

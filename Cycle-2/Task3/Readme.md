#  Task 3: Disease Diagnosis Prediction – Data Science Internship

##  Objective
Build a machine learning model to predict whether a person is diabetic using clinical input features. Provide useful insights for doctors and healthcare screening.

---

##  Dataset

- **Name**: Pima Indians Diabetes Dataset  
- **Source**: [Kaggle Link](https://www.kaggle.com/datasets/uciml/pima-indians-diabetes-database)  
- **Features**: Glucose, BMI, Age, Insulin, BloodPressure, etc.  
- **Target**: 0 = Non-diabetic, 1 = Diabetic  

---

##  Pipeline Steps

### 1. EDA
- Checked for missing/zero values
- Plotted correlations and distributions

### 2. Feature Selection
- Used `SelectKBest` to choose top 6 features

### 3. Preprocessing
- Applied `StandardScaler` for models like SVM

### 4. Models
- Gradient Boosting  
- XGBoost  
- SVM (RBF kernel)

### 5. Evaluation
- Classification report
- AUC-ROC Curve
- Best model: Gradient Boosting with AUC ~0.87

---

##  Key Insights

- High glucose is the strongest signal of diabetes
- Age and BMI increase risk
- Model can be used in hospitals for early flagging

---

##  Tools Used

- Python 3.12  
- pandas, numpy, seaborn, matplotlib  
- scikit-learn, xgboost  

---



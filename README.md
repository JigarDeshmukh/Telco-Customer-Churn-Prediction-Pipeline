# 📊 Telco Customer Churn Prediction Pipeline

## 🚀 Project Overview

This project builds an end-to-end machine learning pipeline to predict **customer churn** using the Telco Customer Churn dataset.

Customer churn prediction helps businesses identify customers who are likely to leave, enabling proactive retention strategies.

---

## 🎯 Objectives

* Analyze customer behavior and identify churn patterns
* Build multiple machine learning models
* Optimize models using GridSearchCV
* Compare performance across models
* Deploy a production-ready prediction pipeline

---

## 🧠 Models Used

* Logistic Regression
* Random Forest
* XGBoost
* Voting Classifier (Ensemble Model)

---

## ⚙️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* XGBoost
* Matplotlib
* Joblib

---

## 🔄 Workflow

### 1. Data Preprocessing

* Handling missing values
* Encoding categorical features
* Feature scaling (where required)
* Column transformation using `ColumnTransformer`

### 2. Model Building

* Built pipelines for each model
* Ensured clean and reusable workflow

### 3. Hyperparameter Tuning

* Used **GridSearchCV** to find best parameters
* Applied cross-validation

### 4. Ensemble Learning

* Combined models using **VotingClassifier**
* Improved prediction performance

### 5. Model Evaluation

* Accuracy Score
* Confusion Matrix
* ROC-AUC Curve
* Classification Report

### 6. Model Deployment

* Saved trained model using `joblib`
* Built prediction pipeline for new data

---

## 📊 Model Evaluation

### Confusion Matrix

Provides a breakdown of:

* True Positives
* False Positives
* True Negatives
* False Negatives

### ROC-AUC Curve

Measures model performance across thresholds:

* AUC close to **1.0 → Excellent model**
* AUC close to **0.5 → Random model**

---

## 📈 Example Prediction

Input:

```python
{
  "gender": "Male",
  "tenure": 12,
  "MonthlyCharges": 70.5,
  ...
}
```

Output:

```python
Churn: Yes / No
```

---

## 💾 How to Run

### 1. Clone Repository

```bash
git clone https://github.com/your-username/telco-churn-prediction.git
```

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run Notebook / Script

### 4. Load Model & Predict

```python
import joblib

model = joblib.load("churn_model.pkl")
prediction = model.predict(new_data)
```

---

## 🚀 Future Improvements

* Deploy using Streamlit / Flask
* Add feature importance visualization
* Build real-time prediction API
* Add dashboard for business insights

---

## 🤝 Conclusion

This project demonstrates a complete machine learning lifecycle — from preprocessing to deployment — and highlights how ML can solve real-world business problems like customer churn.

---

## ⭐ If you like this project

Give it a star ⭐ on GitHub!

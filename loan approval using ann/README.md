# 🏦 Loan Approval Prediction using Artificial Neural Network (ANN)

## 📌 Project Overview

This project predicts whether a loan application will be **Approved** or **Rejected** using an Artificial Neural Network (ANN).

The model analyzes applicant information such as income, education, CIBIL score, loan amount, and asset values to make the prediction.

---

## 📂 Dataset

The dataset contains the following features:

- Number of Dependents
- Education
- Self Employed
- Annual Income
- Loan Amount
- Loan Term
- CIBIL Score
- Residential Asset Value
- Commercial Asset Value
- Luxury Asset Value
- Bank Asset Value

**Target Variable**

- Loan Status (Approved / Rejected)

---

## 🛠 Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- TensorFlow / Keras
- Matplotlib

---

## 🔄 Data Preprocessing

The following preprocessing steps were performed:

- Removed unnecessary column (`loan_id`)
- Checked for missing values
- Encoded categorical features
- Converted target values:
  - Approved → 1
  - Rejected → 0
- Split the data into training and testing sets
- Applied **StandardScaler** to normalize numerical features

---

## 🧠 Model Architecture

The ANN consists of:

- Input Layer (11 Features)
- Hidden Layer: 32 Neurons (ReLU)
- Dropout Layer (0.2)
- Hidden Layer: 16 Neurons (ReLU)
- Output Layer: 1 Neuron (Sigmoid)

Optimizer:
- Adam

Loss Function:
- Binary Crossentropy

Evaluation Metric:
- Accuracy

---

## 📊 Model Performance

### Test Accuracy

**97.78%**

### Confusion Matrix

| Actual / Predicted | Rejected | Approved |
|--------------------|----------|----------|
| Rejected | 323 | 11 |
| Approved | 8 | 512 |

### Classification Report

| Metric | Rejected | Approved |
|---------|----------|----------|
| Precision | 0.98 | 0.98 |
| Recall | 0.97 | 0.98 |
| F1-Score | 0.97 | 0.98 |

The model correctly predicted **835 out of 854 loan applications**, achieving high precision and recall for both classes.

---

## 🚀 Project Workflow

```
Dataset
   │
   ▼
Data Preprocessing
   │
   ▼
Feature Scaling
   │
   ▼
Train-Test Split
   │
   ▼
Build ANN Model
   │
   ▼
Train Model
   │
   ▼
Evaluate Model
   │
   ▼
Predict Loan Status
```

---

## 📈 Future Improvements

- Compare ANN with Logistic Regression, Random Forest, and XGBoost
- Perform Hyperparameter Tuning
- Deploy the model using Streamlit
- Add Explainable AI techniques (SHAP/LIME)

---

## 👨‍💻 Author

**Vinoth G**

- GitHub: https://github.com/vinoth-G18
- LinkedIn: https://linkedin.com/in/vinoth-g18

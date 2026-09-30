# CreditWise Loan System

A machine learning-based loan approval prediction system that analyzes applicant and loan-related information to predict whether a loan application is likely to be **Approved or Rejected**.

## 📌 Project Overview

**CreditWise Loan System** demonstrates an end-to-end machine learning workflow for loan approval prediction, including data preprocessing, exploratory data analysis, feature engineering, model training, and evaluation.

The current implementation is a **machine learning prototype / decision-support system** developed in Jupyter Notebook.

## 🎯 Problem Statement

The system aims to support loan assessment by analyzing applicant factors such as income, credit score, employment status, loan amount, loan term, liabilities, and debt-to-income ratio.

The objective is to build a classification system that predicts whether a loan application is likely to be approved or rejected.

## 🔄 Project Workflow

```text
Dataset → Data Understanding → Data Cleaning → EDA
       → Encoding → Feature Scaling → Feature Engineering
       → Model Training → Evaluation → Model Selection
```

## 🧹 Data Preprocessing

- Dataset inspection
- Missing-value analysis
- Numerical missing-value imputation
- Categorical missing-value imputation
- Removal of `Applicant_ID`
- Categorical encoding
- One-hot encoding
- Feature scaling

## 🔬 Feature Engineering

The project creates:

- `DTI_Ratio_Sq`
- `Credit_Score_Sq`
- `Applicant_Income_log`

## 🤖 Machine Learning Models

- Logistic Regression
- K-Nearest Neighbors (KNN)
- Gaussian Naive Bayes

## 📊 Model Evaluation

Models were evaluated using:

- Precision
- Recall
- F1-Score
- Accuracy
- Confusion Matrix

### Final Results

| Model | Precision | Recall | F1-Score | Accuracy |
|---|---:|---:|---:|---:|
| Logistic Regression | 0.778 | 0.803 | 0.790 | **0.870** |
| KNN | 0.630 | 0.557 | 0.591 | 0.765 |
| Gaussian Naive Bayes | **0.804** | 0.738 | 0.769 | 0.865 |

Because the project prioritizes **precision**, Gaussian Naive Bayes was selected as the final model.

**Final Test Performance:**

- Precision: **80.36%**
- Recall: **73.77%**
- F1-Score: **76.92%**
- Accuracy: **86.50%**

### Confusion Matrix

```text
[[128  11]
 [ 16  45]]
```

## 🛠️ Tech Stack

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## 📁 Project Structure

```text
CreditWise-Loan-System/
│
├── creditwise-loan-system.ipynb
├── README.md
└── dataset/
    └── loan_dataset.csv
```

> Update the dataset path above if your repository uses a different filename or folder structure.

## 🚀 How to Run

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd CreditWise-Loan-System
```

### 2. Install dependencies

```bash
pip install pandas numpy scikit-learn matplotlib seaborn jupyter
```

### 3. Start Jupyter Notebook

```bash
jupyter notebook
```

Open `creditwise-loan-system.ipynb` and run the cells sequentially.

## 🌍 Future Scope

The notebook can be extended into a web-based loan decision-support platform:

```text
Applicant / Bank System
          ↓
      Web Portal
          ↓
       REST API
          ↓
  CreditWise Backend
          ↓
 Preprocessing Pipeline
          ↓
       ML Model
          ↓
   Decision Support
          ↓
    Bank Dashboard
```

Potential future improvements:

- Web-based loan application
- FastAPI/REST API
- Database integration
- Applicant and bank dashboards
- Authentication and authorization
- Model versioning and monitoring
- Explainable predictions
- Audit logging
- Integration with existing banking systems

## ⚠️ Disclaimer

CreditWise is an educational and portfolio machine learning project. The current implementation is a prototype and is **not a production banking or autonomous loan approval system**.

Real-world deployment would require appropriate security, validation, monitoring, governance, fairness assessment, regulatory compliance, and human oversight.

## 👨‍💻 Author

**Aman Sharma**

Data Science & Machine Learning Enthusiast

---

⭐ If you find this project useful, consider giving the repository a star!

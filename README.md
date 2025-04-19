# Predicting-Loan-Approval- (Classification)

This project builds and compares machine learning models to predict whether a loan application will be approved or rejected based on customer and asset information.

---

## 📊 Dataset Overview

- **Source**: Custom Loan Approval Dataset
- **Rows**: 4,269
- **Columns**: 13
- **Target**: `loan_status` → Approved (1) / Rejected (0)

---

## 🧼 Preprocessing

- Dropped `loan_id` (non-informative)
- Handled missing values with median (numeric) and mode (categorical)
- Encoded categorical features with `LabelEncoder`
- No feature scaling needed for tree-based models

---

## 🤖 Models Trained

### 🔹 Logistic Regression (Baseline)

- **Accuracy**: 79.9%
- **F1 Score** (Rejected class): 0.69
- **Confusion Matrix**:

-  ✅ Good baseline but struggles with recall on the rejected class

### 🌲 Random Forest Classifier

- **Accuracy**: 97.8%
- **F1 Score** (Rejected class): 0.97
- **Confusion Matrix**:
- - ✅ Excellent performance, low error rate, handles complex patterns

---

## 📈 Model Comparison

![Confusion Matrix Comparison](confusion_matrices.png)

- Logistic Regression: Higher false negatives/positives  
- Random Forest: More accurate, especially on rejected applications

---

## 🧠 Libraries Used

- Python, Pandas, NumPy
- Scikit-learn: `LogisticRegression`, `RandomForestClassifier`, `LabelEncoder`
- Seaborn, Matplotlib

---

## ✨ Author

**Lokesh Mandarapu** – [LinkedIn](https://linkedin.com/in/mandarapulokesh)

---




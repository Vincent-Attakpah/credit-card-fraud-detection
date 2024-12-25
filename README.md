# credit-card-fraud-detection
# Credit Card Fraud Prediction

A machine learning project to detect fraudulent credit card transactions using feature selection and Random Forest classification.

---

## 📜 Project Description

Credit card fraud is a critical challenge faced by financial institutions. This project implements a predictive model that identifies fraudulent transactions based on anonymized transaction data. It achieves **perfect metrics** (accuracy, precision, recall and F1-score) by leveraging feature engineering and a robust classification model.

---

## 📊 Dataset

- **Source**: The dataset was obtained from [Kaggle's Credit Card Fraud Detection Dataset](https://www.kaggle.com/datasets/mlg-ulb/creditcardfraud).
- **Description**:
  - 31 columns: anonymized features (`V1`–`V28`), `Amount`, and `Class` (0 = non-fraud, 1 = fraud).
  - 398,041 training samples, 170,589 test samples.

---

## ⚙️ Methodology

1. **Exploratory Data Analysis (EDA)**:
   - Analyzed data distribution, class imbalance, and feature correlation.
2. **Feature Engineering**:
   - Scaled the `Amount` column using log transformation.
   - Applied **PCA** to reduce dimensionality.
   - Selected the top 10 features using `SelectKBest` with the chi-squared test.
3. **Modeling**:
   - Used a Random Forest Classifier with hyperparameter tuning.
4. **Evaluation**:
   - Achieved 100% accuracy on the test set.

---

## 📈 Results

| Metric       | Value |
|--------------|-------|
| **Accuracy** | 1.00  |
| **Precision**| 1.00  |
| **Recall**   | 1.00  |
| **F1-Score** | 1.00  |

The confusion matrix shows perfect classification for both fraudulent and non-fraudulent transactions.

---

## 🛠️ Requirements

Install the required Python packages before running the project:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn

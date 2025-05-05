# Customer Churn Prediction Models

This repository contains multiple machine learning models developed to predict **customer churn** using a real-world dataset. Built as part of the **Kodessphere Hackathon 2024**, the project explores different algorithms, evaluates their performance, and draws insights to support customer retention strategies.

---

## 🌟 Hackathon Project

**🏆 Team Name**: Nova
**📅 Date**: March 2024
**🌐 Event**: Kodessphere Hackathon 2024
**📍 Goal**: Predict customer churn with high recall and actionable insights for telecom service providers.

---

## Project Structure

```
.
├── dataset/
│   └── telecom_churn_data.csv
├── models/
│   ├── logistic_regression_model.ipynb
│   ├── decision_tree_model.ipynb
│   ├── random_forest_model.ipynb
├── results/
│   ├── confusion_matrices/
│   └── classification_reports/
├── README.md
└── assets/
    └── demo-thumbnail.png (optional)
```

---

## Dataset

* Format: CSV
* Records: 2,321 customers
* Features: Includes usage metrics, contract details, payment info, etc.
* Target: `Churn` (binary classification – 0: Non-churn, 1: Churn)

---

## Models Used

1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**

Each model was trained and evaluated using:

* Train/Test split
* Confusion Matrix
* Classification Report (Precision, Recall, F1-score)
* Accuracy Score

---

## Performance Summary (for one algorithm)

| Model               | Accuracy | Recall (Churn) | Precision (Churn) | F1-score (Churn) |
| ------------------- | -------- | -------------- | ----------------- | ---------------- |
| Logistic Regression | \~63%    | \~62%          | \~38%             | \~47%            |
| Decision Tree       | \~67%    | \~60%          | \~41%             | \~49%            |
| Random Forest       | **65%**  | **66%**        | **40%**           | **49%**          |

> The Random Forest model achieved the best balance between identifying churners and minimizing false positives.

---

## Confusion Matrix (Random Forest)

```
[[1102  609]
 [ 210  400]]
```

## Conclusion

* The models offer moderate accuracy but strong **recall for churners**, making them useful for **early detection**.
* Random Forest shows the best overall balance.
* Future improvements:

  * Feature engineering
  * Handling class imbalance (e.g., SMOTE)
  * Trying ensemble methods like XGBoost or LightGBM

---

## Requirements

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

##  Team Nova

* Devanshi S
* Maithali B. 
* Aditya Bahadur @abahadur29

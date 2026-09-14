# 📊 Customer Churn Prediction

## 📝 Project Overview

This project focuses on predicting **customer churn** using Machine Learning. The main goal is to identify customers who are likely to leave a service and compare different classification models to find the best-performing model.

In this project, I compared a **Decision Tree** with a **Random Forest**, performed **5-Fold Cross-Validation**, and applied **hyperparameter tuning** to improve model performance.

---

## 🎯 Objectives

- 🌳 Build a Decision Tree baseline model
- 🌲 Build a Random Forest model
- 📈 Compare model performance using different evaluation metrics
- 🔄 Perform 5-Fold Cross-Validation
- ⚙️ Tune Random Forest hyperparameters
- 🏆 Select the best-performing final model
- 📄 Generate a Kaggle-style `submission.csv` file

---

## 🤖 Models Used

### 🌳 Decision Tree
A Decision Tree was used as the baseline model for predicting customer churn.

### 🌲 Random Forest
Random Forest combines multiple decision trees and uses their predictions to improve generalization.

### ⚙️ Tuned Random Forest
Hyperparameter tuning was performed on the Random Forest to find a better-performing configuration.

---

## 📏 Evaluation Metrics

The models were evaluated using:

- 🎯 Accuracy
- 🔍 Precision
- 📌 Recall
- ⭐ F1-Score

Since the churn dataset is imbalanced, **Recall and F1-Score** were given particular importance because detecting actual churners is an important business objective.

---

## 🔄 Cross-Validation

I used **5-Fold Cross-Validation** to obtain a more reliable estimate of model performance.

Cross-validation evaluates the model on multiple train/test splits instead of relying on a single split, helping us understand how consistently the model performs on different subsets of the data.

---

## 🏆 Final Model

The **Tuned Random Forest** was selected as the final model.

| Metric | Score |
|---|---:|
| 🎯 Accuracy | 0.805 |
| 🔍 Precision | 0.662 |
| 📌 Recall | 0.540 |
| ⭐ F1-Score | 0.595 |

The Tuned Random Forest achieved the **highest F1-score** among the final compared models and provided the best overall performance for this churn prediction task.

---

## 📊 Model Comparison

| Model | Accuracy | Precision | Recall | F1-Score |
|---|---:|---:|---:|---:|
| 🌳 Decision Tree | 0.794 | 0.631 | 0.540 | 0.582 |
| 🌲 Random Forest | 0.795 | 0.643 | 0.511 | 0.569 |
| ⚙️ Tuned Random Forest | **0.805** | **0.662** | 0.540 | **0.595** |

---

## 💡 Key Findings

- 🌳 The Decision Tree performed better than the default Random Forest in F1-Score.
- ⚙️ Hyperparameter tuning improved the Random Forest's overall performance.
- 🏆 The Tuned Random Forest achieved the highest F1-Score of **0.595**.
- 📌 Recall was **0.540**, meaning the model still misses some actual churners.
- ⚠️ Class imbalance remains an important limitation.

---

## 🚀 Future Improvements

If more time were available, I would:

- ⚖️ Handle class imbalance using `class_weight='balanced'` or SMOTE
- 🤖 Try additional models such as Logistic Regression, Gradient Boosting, and XGBoost
- ⚙️ Perform deeper hyperparameter tuning
- 🛠️ Apply additional feature engineering
- 📈 Further optimize the model for better churn detection

---

## 📁 Project Files

```text
Customer-Churn-Prediction/
│
├── 📓 ml-lab4-machine-learning-models.ipynb
└── 📖 README.md

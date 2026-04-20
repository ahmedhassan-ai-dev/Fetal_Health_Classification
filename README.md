# Fetal Health Classification: Predict & Protect 🏥

## 📌 Project Overview
This project aims to classify fetal health into three categories (**Normal, Suspect, or Pathological**) using Cardiotocogram (CTG) data. The goal is to provide a predictive tool that can help healthcare professionals identify high-risk cases early, potentially saving lives.

## 📊 Dataset Highlights
The dataset consists of features extracted from CTG exams. 
- **Target Variable:** `fetal_health` (1: Normal, 2: Suspect, 3: Pathological)
- **Problem Type:** Multi-class Classification.

## ⚙️ Methodology & Models
We explored several classification algorithms to find the most robust predictor:
* **Logistic Regression:** Baseline multinomial classification.
* **K-Nearest Neighbors (KNN):** Our top-performing model.
* **Gaussian Naive Bayes (GNB):** Probabilistic approach.
* **Support Vector Classifier (SVC):** Kernel-based separation.



## 📈 Model Performance & Evaluation
While accuracy is important, in healthcare, **Recall** and **ROC-AUC** are crucial to avoid missing any "Pathological" cases.

### Best Model: K-Nearest Neighbors (KNN)
| Metric | Score |
| :--- | :--- |
| **Train Accuracy** | 96.47% |
| **Test Accuracy** | 94.11% |
| **Mean CV Accuracy** | 92.94% |
| **ROC-AUC Score** | **0.988** |

## 🛠️ Key Takeaways
- **KNN** outperformed other models, showing excellent generalization with a high ROC-AUC.
- The high **F2-Score** (prioritizing Recall) ensures the model is sensitive enough to detect health risks effectively.


# 📟 Semiconductor Yield Prediction using Sensor Signal Analysis

### 🔬 Domain: Semiconductor Manufacturing Process

### 📁 Dataset: `sensor-data.csv` (1567 samples × 591 features)

### 🎯 Objective: Classify Pass/Fail Yield & Identify Most Relevant Features

---

## 🧠 Overview

In a modern semiconductor fabrication line, hundreds of sensors continuously monitor various process steps to ensure quality and efficiency. However, not every signal captured from these sensors is meaningful — some are irrelevant or simply noisy.

This project applies machine learning and feature selection techniques to:

* Predict whether a manufactured unit passes or fails internal testing.
* Identify and retain only the most critical features (signals) that impact yield quality.
* Improve process understanding by surfacing key contributors to yield excursions.

---

## 📊 Dataset Description

* **File**: `sensor-data.csv`
* **Rows**: 1567 production units (samples)
* **Columns**:

  * `591` sensor-derived features (continuous values)
  * `Target`:

    * `-1` → Pass
    * `1` → Fail
* **Nature**: High-dimensional, unlabeled features with a binary classification target.

---

## 🎯 Project Goals

1. Build a robust **binary classifier** (Pass vs. Fail) using sensor data.
2. Apply **feature selection techniques** to filter out redundant/noisy signals.
3. Analyze which features contribute the most to prediction performance.
4. Optimize for **accuracy, precision, recall**, and **interpretability**.
5. Evaluate whether a reduced set of features maintains performance.

---

## 🛠️ Techniques Used

* Exploratory Data Analysis (EDA)
* Feature Selection:

  * Variance Thresholding
  * Mutual Information
  * Recursive Feature Elimination (RFE)
  * Tree-based Importance (Random Forest, Gradient Boosting)
* Machine Learning Models:

  * Logistic Regression
  * Random Forest
  * Gradient Boosting
  * Support Vector Machine (SVM)
* Cross-validation and Hyperparameter Tuning
* Model Evaluation Metrics:

  * Accuracy, Precision, Recall, F1-score
  * Confusion Matrix, ROC-AUC

---

## 📈 Results Summary

Feature selection successfully removed unnecessary signals, reducing noise and improving overall model efficiency. To address the inherent class imbalance in the dataset, SMOTE (Synthetic Minority Over-sampling Technique) was applied, resulting in more balanced training and better generalization. Among the models evaluated, Random Forest outperformed others after thorough hyperparameter tuning, delivering the best combination of accuracy, robustness, and interpretability. The final trained model is now capable of reliably predicting semiconductor yield failures, providing valuable insights for process engineers and contributing to reduced production costs and improved throughput.

---

## 💡 Key Learnings

* High-dimensional sensor data often contains **redundant signals**.
* **Feature selection not only improves performance** but also enhances **interpretability and efficiency**.
* Even in complex manufacturing systems, data-driven models can aid engineers in identifying **critical process parameters** influencing yield.

---


## 👨‍🔬 Author

**Jawad Parkar**


---


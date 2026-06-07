## Predictive-Modeling-for-Agriculture
Built an ML model to identify the most important soil nutrient for crop prediction. Used Logistic Regression to predict optimal crop types based on Nitrogen (N), Phosphorus (P), Potassium (K), and pH levels, and evaluated feature importance using macro F1-scores.

### Project Overview

Selecting the right crop based on soil conditions is critical for maximizing agricultural productivity. However, measuring all soil properties can be costly and time-consuming for farmers.

This project uses machine learning to determine which soil feature provides the strongest predictive power for identifying the optimal crop to grow.

The analysis was conducted using Logistic Regression on a multiclass crop classification dataset containing soil nutrient measurements.

---

### Dataset

The dataset contains 2,200 observations and the following variables:

* **N** – Nitrogen content ratio in soil
* **P** – Phosphorous content ratio in soil
* **K** – Potassium content ratio in soil
* **pH** – Soil pH value
* **crop** – Optimal crop for the given soil conditions (target variable)

The dataset includes 22 different crop categories.

---

### Objectives

1. Build a multiclass classification model to predict crop type.
2. Evaluate predictive performance using classification metrics.
3. Identify the single most important soil feature for crop prediction.

---

### Methodology

### Data Preparation

* Loaded dataset using Pandas
* Checked for missing values
* Defined feature matrix (X) and target variable (y)
* Split data into training and testing sets (80:20)

### Model Development

Implemented Logistic Regression for multiclass classification.

### Model Evaluation

Evaluated performance using:

* Accuracy Score
* Classification Report
* Confusion Matrix
* Macro F1-Score

### Feature Importance Analysis

Trained separate Logistic Regression models using individual features:

* Nitrogen (N)
* Phosphorous (P)
* Potassium (K)
* pH

Compared their Macro F1-Scores to determine the strongest predictor.

---

### Results

| Feature | Macro F1 Score |
| ------- | -------------- |
| N       | 0.105          |
| P       | 0.139          |
| K       | 0.211          |
| pH      | 0.047          |

### Best Predictive Feature

**Potassium (K)** achieved the highest Macro F1 Score:

K → 0.2109

This suggests that Potassium content is the most informative single soil measurement for predicting the optimal crop in this dataset.

---

### Key Findings

* Potassium (K) was the strongest individual predictor of crop type.
* pH showed the weakest predictive performance among the available features.
* Using only a single soil measurement significantly limits predictive accuracy, indicating that crop selection depends on a combination of soil characteristics.

---

### Technologies Used

* Python
* Pandas
* Scikit-learn
* Logistic Regression
* Jupyter Notebook

---

### Author

Unnati Rai
B.Sc. Economics SSE(Data Analytics Specialization)

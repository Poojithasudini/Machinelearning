# Heart Disease Prediction using Machine Learning

## Overview

This project builds a machine learning system to predict the likelihood of heart disease based on patient health data. The goal is to compare multiple models, evaluate their performance, and identify the most reliable approach for prediction.

The workflow covers data preprocessing, model training, evaluation, and basic explainability.

---

## Dataset

The dataset used in this project is the **Heart Disease UCI dataset**, which contains medical attributes such as age, cholesterol levels, chest pain type, and more.

Each row represents a patient, and the target variable indicates whether heart disease is present.

---

## Project Workflow

### 1. Data Preparation

* Cleaned column names for consistency
* Checked for missing values
* Converted target variable into binary format when required

### 2. Feature Processing

* Separated features and target variable
* Encoded categorical variables using label encoding
* Applied scaling and imputation using a preprocessing pipeline

### 3. Model Building

The following machine learning models were implemented:

* Logistic Regression
* Random Forest
* Support Vector Machine (SVM)
* K-Nearest Neighbors (KNN)
* XGBoost (if available)

Each model was trained using a consistent pipeline for fair comparison.

---

## Evaluation Metrics

Models were evaluated using:

* Accuracy
* Precision
* Recall
* F1 Score
* ROC-AUC

Recall was given special importance since missing a positive heart disease case can be critical.

---

## Results

All models were compared, and the best-performing model was selected based on recall score.

In most cases, **Random Forest** performed best due to its ability to handle complex relationships in the data.

---

## Feature Importance

For tree-based models, feature importance was analyzed to understand which variables contributed most to predictions.

This helps in interpreting the model and identifying key health indicators.

---

## Model Explainability

SHAP (SHapley Additive exPlanations) was used to provide insights into how features influence predictions.

This adds transparency to the model, which is especially important in healthcare applications.

---

## Sample Prediction

The project includes a sample prediction using median values of features to demonstrate how the trained model can be used for new data.

---

## Technologies Used

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib
* XGBoost (optional)
* SHAP (optional)
* Google Colab

---

## How to Run

1. Open the project in Google Colab
2. Upload the dataset file (`heart_disease_uci.csv`)
3. Run all cells sequentially
4. View model results and visualizations

---

## Future Improvements

* Add advanced feature engineering
* Handle class imbalance using SMOTE or similar techniques
* Perform hyperparameter tuning for better performance
* Deploy the model using a web interface (e.g., Streamlit)

---

## Disclaimer

This project is for educational purposes only. It should not be used as a medical diagnostic tool.

---

## Author

Developed as part of a machine learning practice project.

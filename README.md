# Breast Cancer Classification using Logistic Regression

## Summary of the Code
This project builds a **breast cancer classification model** using the **Wisconsin Breast Cancer Dataset** from Kaggle. The dataset is preprocessed, standardized, and used to train a **Logistic Regression** model for classification.

## Steps Involved

###  Dataset Download
- The dataset is downloaded using the `kagglehub` library.
- `pandas` is used to load the dataset.

###  Data Preprocessing
- Unnecessary columns (`Unnamed: 32` and `id`) are removed.
- The `diagnosis` column is encoded:
  - **Malignant (M) → 1**
  - **Benign (B) → 0**
- A **bar chart** is plotted to show the class distribution.

###  Feature Selection & Splitting
- **Predictors (`X`)**: All columns starting from `'radius_mean'`.
- **Target (`Y`)**: The `diagnosis` column.
- **Feature Standardization**: `StandardScaler` is used to scale the features.
- The dataset is split into **training (67%)** and **testing (33%)**.

###  Model Training & Evaluation
- A **Logistic Regression model** is trained on `X_train` and `y_train`.
- Predictions are made on `X_test`.
- The model is evaluated using:
  - **Accuracy Score** (`accuracy_score`)
  - **Classification Report** (`classification_report`)

---

## Installation & Usage

### 🔹 Install Required Libraries
```bash
pip install kaggle kagglehub pandas seaborn scikit-learn 

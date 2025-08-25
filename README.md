## Genomic Cancer Prediction

### Project Overview

This project aims to predict the **presence of cancer** based on the expression levels of two genes. By analyzing the numerical values of 'Gene One' and 'Gene Two', the goal is to develop a machine learning model that can accurately classify whether a given sample indicates the presence of cancer. This type of genomic analysis is a foundational task in bioinformatics and medical diagnostics.

-----

### Technical Highlights

  * **Dataset**: The dataset used is `gene_expression.csv`, which contains simulated gene expression data.
  * **Size**: 3000 entries, 3 columns.
  * **Key Features**:
      * `Gene One` and `Gene Two` (numerical expression levels).
  * **Approach**:
      * **Data Cleaning**: The dataset was used as-is, as no missing values were present. Duplicate rows were identified but not dropped in the provided code, which might affect model training and evaluation.
      * **Exploratory Data Analysis**: The code checks basic statistics like shape, size, info, descriptive statistics, and unique values.
      * **Binary Classification**: The target variable `Cancer Present` is a binary outcome (0 or 1).
      * **Models Used**:
          * Logistic Regression, Ridge Classifier, SVC, Random Forest, XGBoost, AdaBoost, Gradient Boosting, Bagging, Decision Tree.
  * **Best Accuracy**:
      * **94.3%** with SVC.
      * **93.0%** with Gradient Boosting Classifier.
      * **92.3%** with AdaBoost Classifier.
      * The high accuracies for ensemble models suggest that the combination of gene expression levels provides strong discriminative power for predicting cancer.

-----

### Purpose and Applications

  * **Assist in the genomic diagnosis of cancer** by analyzing gene expression data.
  * Serve as a tool for researchers to identify potential biomarkers for cancer.
  * Provide a foundational model for developing more complex multi-gene panel diagnostics.
  * Demonstrate the application of machine learning in personalized medicine and bioinformatics.

-----

### Installation

Clone the repository and extract the data from the zip file.

Install the necessary libraries:

```bash
pip install pandas numpy seaborn matplotlib scikit-learn xgboost
```

-----

### Collaboration

We welcome contributions to improve the project. You can help by:

  * Handling the duplicate rows by either dropping them or investigating their significance.
  * Performing comprehensive hyperparameter tuning and cross-validation for all models to ensure robustness.
  * Exploring the use of dimensionality reduction or feature engineering if more genes were to be added to the dataset.
  * Adding explainability (e.g., SHAP or LIME) to understand which of the two genes is a stronger predictor of cancer.

# Concrete Compressive Strength Prediction and Classification 🏗️

This project involves predicting the concrete compressive strength and classifying concrete recipes based on their strength. The dataset includes concrete mixture ingredients and their curing age. The goal is to predict the **Concrete Compressive Strength** for the regression model and classify the strength into categories for the classification model.

## Project Overview 🚀

### Tasks:

1. **Regression Model**: Predict the concrete compressive strength using the ingredients and curing age.
2. **Classification Model**: Categorize the concrete based on its compressive strength into predefined classes.

Both models will be evaluated using multiple conventional machine learning algorithms and deep learning techniques.

## Data Explanation 📊

The dataset contains information on various ingredients and the curing age of concrete mixtures, along with their compressive strength. The goal is to predict the **Concrete Compressive Strength** based on these features.

### Variables 📑

| **Variable Name**               | **Data Type** | **Measurement**        | **Description**                                               |
|----------------------------------|---------------|------------------------|---------------------------------------------------------------|
| Cement              | Quantitative  | kg in a m³ mixture     | Amount of cement in the concrete mixture.                     |
| Blast Furnace Slag  | Quantitative  | kg in a m³ mixture     | Amount of blast furnace slag in the concrete mixture.         |
| Fly Ash           | Quantitative  | kg in a m³ mixture     | Amount of fly ash in the concrete mixture.                    |
| Water             | Quantitative  | kg in a m³ mixture     | Amount of water in the concrete mixture.                      |
| Superplasticizer  | Quantitative  | kg in a m³ mixture     | Amount of superplasticizer in the concrete mixture.           |
| Coarse Aggregate   | Quantitative  | kg in a m³ mixture     | Amount of coarse aggregate in the concrete mixture.           |
| Fine Aggregate     | Quantitative  | kg in a m³ mixture     | Amount of fine aggregate in the concrete mixture.             |
| Age                              | Quantitative  | Day (1~365)            | Number of days the concrete mixture has cured.                |
| Concrete Compressive Strength    | Quantitative  | MPa                    | Output variable: The compressive strength of the concrete.     |

### Data Characteristics:

- **Number of Instances (Observations)**: 1030
- **Number of Attributes**: 9 (8 input variables and 1 output variable)
- **Missing Values**: None, the dataset is complete.
- **Data Format**: Raw, unscaled data. All variables are quantitative.

## Model Results 📈

### Regression Model (Concrete Strength):

- **Deep Learning Model**:
  - R-squared: 0.88
  - RMSE: 5.54
- **Best Traditional Model**: XGBoost Regressor
  - R-squared: 0.93
  - RMSE: 4.30

### Classification Model (Concrete Class):

- **Deep Learning Model**:
  - Accuracy: 79.6%
- **Best Traditional Model**: Random Forest Classifier
  - Accuracy: 88.8%

## Performance Comparison ⚙️

### Classification Models (Accuracy):

| **Model**                          | **Accuracy** |
|-------------------------------------|--------------|
| Random Forest Classifier           | 88.8%        |
| Gradient Boosting Classifier       | 88.3%        |
| Decision Tree Classifier           | 83.9%        |
| Logistic Regression                | 80.1%        |
| KNeighbors Classifier              | 73.3%        |
| Gaussian Naive Bayes              | 67.9%        |
| Bernoulli Naive Bayes             | 64.6%        |

### Regression Models (R-squared, RMSE, MAE):

| **Model**                 | **R-squared** | **RMSE** | **MAE**   |
|---------------------------|---------------|----------|-----------|
| XGBoost Regressor         | 0.93          | 4.30     | 2.78      |
| Gradient Boosting         | 0.90          | 5.05     | 3.69      |
| Decision Tree Regressor   | 0.86          | 6.10     | 3.81      |
| Extra Tree                | 0.83          | 6.61     | 4.13      |
| Ridge                     | 0.81          | 7.06     | 5.45      |
| Linear                    | 0.81          | 7.07     | 5.48      |
| KNeighbors Regressor      | 0.74          | 8.23     | 6.46      |
| Lasso                     | 0.69          | 8.96     | 6.77      |
| ElasticNet                | 0.65          | 9.49     | 7.39      |

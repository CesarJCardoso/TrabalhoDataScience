# Wine Quality Prediction and Malic Acid Regression

![wine-glass](https://cdn.discordapp.com/attachments/837027141953650688/1165383475105370193/toppng.com-bouteille-et-verre-de-vin-rouge-png-glass-red-wine-580x470.png?ex=6546a6f0&is=653431f0&hm=3766695b0db2fb5d4de4fc54cbc107d09c9457762e78c25a9867eaec987182ac&)

This project leverages the `wine.csv` dataset for two analytical tasks:
1. **Wine Quality Prediction (Classification)**: Utilizing various chemical properties to predict the wine class.
2. **Malic Acid Prediction (Regression)**: Estimating the malic acid content in wine based on other chemical characteristics.

## Dataset Overview

The dataset comprises various chemical attributes of wine samples. It includes the following key columns:

- `Class`: The target variable for the classification task.
- `Alcohol`: The alcohol content in the wine.
- `Malic Acid`: Used as a feature in the classification model and as the target in the regression model.
- Additional chemical properties like `Ash`, `Alcalinity of Ash`, `Magnesium`, `Total Phenols`, `Flavanoids`, `Nonflavanoid Phenols`, `Proanthocyanins`, `Color Intensity`, `Hue`, `OD280/OD315 of Diluted Wines`, and `Proline`.

## Classification Model (Wine Quality Prediction)

For the classification task, a Random Forest model is employed.

### Features Used
- All available columns, except 'Class' since its the target

### Model Description
- **Model**: Random Forest Classifier

### Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1 Score
- AUC (Area Under the Curve)

## Regression Model (Malic Acid Prediction)

The regression task is addressed using Ridge Regression.

### Features Used
- All columns except 'Malic Acid'.

### Model Description
- **Model**: Ridge Regression

### Evaluation Metrics
- Mean Squared Error (MSE)
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Normalized Mean Absolute Error (NMAE)
- R² Score

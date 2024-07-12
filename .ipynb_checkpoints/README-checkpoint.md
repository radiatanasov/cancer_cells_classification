# Cancer Cell Classification

This project uses the "Cancer_Data.csv" dataset, which includes 570 observations of cancer cells with 30 features for each cell. Each observation is labeled as either benign or malignant, with benign cells labeled "B" and malignant cells labeled "M". [Dataset on Kaggle](https://www.kaggle.com/datasets/erdemtaha/cancer-data?select=Cancer_Data.csv).

## Contents

- [Description](#description)
- [Dataset Information](#dataset-information)
- [Libraries Used](#libraries-used)
- [Data Exploration](#data-exploration)
- [Data Preparation](#data-preparation)
- [Models and Techniques](#models-and-techniques)
- [Performance Evaluation](#performance-evaluation)
- [Model Interpretation](#model-interpretation)
- [Contact](#contact)

## Description

The goal of this project is to classify cancer cells as either benign or malignant based on their physical characteristics using various machine learning models. The project explores different models and techniques to improve classification accuracy and interpretability.

## Dataset Information

The dataset includes 570 observations of cancer cells, with the following features recorded for each cell:

- **id**: Unique identifier for each patient in the database
- **diagnosis**: Whether the cancer cell is benign (B) or malignant (M)
- **radius_mean**: Mean cell radius
- **texture_mean**: Average cell texture
- **perimeter_mean**: Average cell perimeter
- **area_mean**: Average cell area
- **smoothness_mean**: Average cell smoothness
- **compactness_mean**: Average cell compactness
- **concavity_mean**: Median cell concavity
- **concave points_mean**: The average number of concave points of the cell
- **symmetry_mean**: Mean cell symmetry
- **fractal_dimension_mean**: Average fractal dimension of the cell
- **radius_se**: The standard deviation of the cell radius
- **texture_se**: The standard deviation of the cell texture
- **perimeter_se**: The standard deviation of the cell perimeter
- **area_se**: The standard deviation of the cell area
- **smoothness_se**: The standard deviation of cell smoothness
- **compactness_se**: The standard deviation of cell compactness
- **concavity_se**: The standard deviation of the concavity of the cell
- **concave points_se**: The standard deviation of the number of indented points of the cell
- **symmetry_se**: The standard deviation of cell symmetry
- **fractal_dimension_se**: The standard deviation of cell symmetry
- **radius_worst**: The largest dimension of the cell radius
- **texture_worst**: The largest dimension of the cell texture
- **perimeter_worst**: The largest dimension of the cell perimeter
- **area_worst**: The largest dimension of the cell area
- **smoothness_worst**: The greatest smoothness of the cell
- **compactness_worst**: The greatest compactness of the cell
- **concavity_worst**: The greatest concavity of the cell
- **concave points_worst**: Points of greatest concavity
- **symmetry_worst**: The degree of symmetry of the cancer cell
- **fractal_dimension_worst**: The fractal dimension of the cell

## Libraries Used

- pandas
- numpy
- matplotlib
- seaborn
- sklearn

## Data Exploration

Initial data exploration includes examining the structure of the dataset, checking for missing values, performing preliminary data analysis, and analyzing the distribution of the features.

## Data Preparation

To prepare the data, the following steps were taken:

Remove the "diagnosis" column: This column contains the target variable, so we need to separate it into a separate variable. We can detach it by saving it to a new variable and removing it from the original DataFrame.
Split the data: The dataset is split into training and test sets in an 80:20 ratio.
Standardize the data: The StandardScaler class from the sklearn.preprocessing library is used to standardize (normalize) the data in X_train and X_test. Standardization ensures that all features have the same scale.

## Models and Techniques

The following models were used in this project:

1. Logistic Regression (Default model)
2. Logistic Regression (Tuned model)
3. Decision Tree (Default model)
4. Decision Tree (Tuned model)
5. Random Forest (Default model)
6. Random Forest (Tuned model)
7. Multi-layer Perceptron (MLP) Classifier

## Performance Evaluation

The performance of the models was evaluated using various metrics, including AUC, balanced accuracy, sensitivity, and specificity.

## Model Interpretation

The models were interpreted using various techniques, including:

Precision-Recall Curve: For the Tuned Random Forest model.
Logistic Regression Coefficients: To understand the importance of features in the Logistic Regression model.
SHAP Summary Plot: To visualize feature importance and the impact of each feature on the predictions.

## Contact

If you have any questions or suggestions, you can contact me at radi2035@gmail.com.
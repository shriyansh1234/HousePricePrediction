## Overview
This project aims to predict house prices based on a dataset obtained from Kaggle. The data is imported as an Excel file and undergoes a thorough data cleaning and analysis process. Two regression models, k-Nearest Neighbors (KNN) and Random Forest, are employed to predict house prices. The analysis includes data imputation, outlier removal, visualization of correlations, and model comparison.

## Dataset
The dataset used in this project is sourced from Kaggle and is provided in Excel format. The data contains information on various factors that may influence house prices.

## Data Cleaning
The data cleaning process involves several steps:
- Imputation: Missing values in columns with at least 50% values are imputed.
- Removal: Columns with 100% missing values are removed.
- Outlier Handling: Outliers are identified and removed from the dataset.
- Categorization: Different types of housing/buildings are separated into their own categories for more granular analysis.

## Exploratory Data Analysis (EDA)
EDA is performed to understand the relationships between different factors and house prices. Correlation matrices and visualizations are used to identify patterns and insights.

## Data Splitting
To evaluate model performance, the dataset is split into an 80/20 ratio for training and testing. This ensures that the models are tested on unseen data to assess their generalization capabilities.

## Models Used
We explored two regression models for our house price prediction task:

1. **k-Nearest Neighbors (KNN) Regression**
KNN, an instance-based learning approach, averages the values of k-nearest neighbors to predict the target variable. Despite its simplicity, KNN struggled to handle the complexity and noise inherent in our dataset.

2. **Random Forest Regression**
Random Forest Regression, an ensemble learning method, outperformed KNN in our evaluation. Leveraging bootstrapping and boosting techniques, Random Forest demonstrated robustness and accuracy in capturing complex relationships within the data.

### Decision Rationale
The decision to favor Random Forest over KNN was driven by its superior performance, especially in generalizing to unseen data. Random Forest's ensemble nature and ability to handle noise and high dimensionality aligned well with the challenges posed by our house price prediction task. In summary, Random Forest Regression was chosen for its reliability, accuracy, and adaptability to the intricacies of our dataset.

## Conclusion
In conclusion, the Random Forest Regression model is chosen as the better fit for predicting house prices in this specific context. The analysis and code for this project are available in the repository.

# Data Preparation and Engineering for Housing Data

## Project Overview
This repository hosts the implementation and findings of the CSC3831 assignment focusing on Data Preparation and Engineering. The project comprises two primary tasks: outlier detection and data imputation, utilizing both non-algorithmic and algorithmic methods for a comprehensive analysis. 

## Objectives
- **Outlier Detection**: Identify and analyze outliers in housing data through both non-algorithmic and algorithmic approaches.
- **Data Imputation**: Evaluate the efficacy of KNN and MICE imputation methods on housing data with simulated missing values.

## Data
The dataset, `houses.csv`, represents various housing characteristics and is used to identify outliers and impute missing data. Exploratory Data Analysis (EDA) provided insights into the dataset's distribution, variability, and potential outliers.

## Methodologies
### Outlier Detection
- **Non-Algorithmic Detection**: Utilized statistical methods and visual inspection to identify outliers based on the Interquartile Range (IQR) method.
- **Algorithmic Detection**: Applied the Local Outlier Factor (LOF) to automate the identification of outliers, utilizing Python's Scikit-learn library.

### Data Imputation
- **KNN Imputation (M1)**: Imputed missing data using the K-Nearest Neighbors approach to prepare for regression modeling.
- **MICE Imputation (M2)**: Employed Multiple Imputation by Chained Equations to handle missing data, aiming to assess its impact on model accuracy.

## Implementation and Analysis
The project was implemented in Python, with analysis and modeling conducted in Jupyter Notebooks (`Code.ipynb`). Detailed analysis, including statistical summaries, visualizations, and model evaluations, are documented within the notebook and the `OUTLIER DETECTION.pdf`.

- The analysis revealed significant variability and outliers across features such as `median_house_value`, `total_rooms`, and `population`.
- Comparative analysis between non-algorithmic and algorithmic outlier detection methods highlighted their respective benefits and detriments.
- Regression models M1 and M2 were developed to assess the performance of KNN and MICE imputation methods. Model performance was evaluated based on Mean Squared Error (MSE) and R-squared values, with graphical analysis providing further insights.

## Results
- Outlier detection methods identified key features with significant outliers, influencing the subsequent imputation and modeling phases.
- Both KNN and MICE imputation methods prepared the dataset effectively for regression analysis, with subtle differences in model performance.
- Comparative evaluation suggested a slightly better performance of the KNN imputation (M1) over MICE (M2), though differences were marginal.

## Running the Project
Ensure Python and necessary libraries (Pandas, Numpy, Scikit-learn) are installed. Run the Jupyter Notebook (`Code.ipynb`) for a step-by-step walkthrough of the analysis, including data preprocessing, outlier detection, imputation, and regression modeling.


## Acknowledgments
- CSC3831 Course Instructors and TAs for providing the dataset and guidance.
- Scikit-learn, Pandas, and Numpy documentation for implementation references.

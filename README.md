# Predicting Stroke Occurrence: An Applied Machine Learning Approach

## School of Science & Technology  
### Department of Computer Science  
#### City, University of London

---

The majority of brain strokes are caused by an unanticipated obstruction of the heart's and brain's regular operations. Researchers can use a variety of machine learning techniques to forecast the likelihood of a stroke occurring. This project studies the use of machine learning techniques to predict the long-term outcomes of stroke victims. By developing and analyzing several machine learning models, we can accurately predict strokes, which is crucial for early treatment. The dataset included 5110 observations of patients who had suffered a stroke and their modifiable risk factors.

*Keywords: Stroke, predictive analytics, brain, machine learning, data analysis*

## Table of Contents
1. [Introduction](#introduction)
2. [Analysis Plan](#analysis-plan)
3. [Data](#data)
4. [Analysis](#analysis)
   - [Data Preparation](#data-preparation)
   - [Data Exploration and Analysis](#data-exploration-and-analysis)
   - [Data Pre-processing](#data-pre-processing)
   - [Machine Learning Models](#machine-learning-models)
5. [Results and Reflections](#results-and-reflections)
6. [References](#references)

---

## Introduction
In the UK, strokes occur every five minutes, affecting 100,000 people annually. Stroke is the second leading cause of death worldwide. The World Health Organization (WHO) estimates that 17.7 million people died from cardiovascular illnesses in 2017, with 6.7 million of those deaths attributable to stroke. Factors such as age, body mass index, smoking status, average glucose level, hypertension, heart disease, and body mass index are critical risk factors for stroke. This study uses the "healthcare-dataset-stroke-data" from Kaggle, which includes 5110 observations and 12 attributes, to predict stroke occurrence.

## Analysis Plan
Our analysis focuses on understanding the factors leading to stroke, the correlations between attributes, and identifying the most suitable model for prediction. The following steps outline our plan:

1. **Identify key risk factors for stroke.**
2. **Investigate the dataset and formulate hypotheses.**
3. **Develop and apply machine learning models.**
4. **Critically evaluate different models for accuracy.**

## Data
The dataset, sourced from Kaggle, includes 5110 observations with 12 attributes, such as age, gender, marital status, patient identifier, work type, residence type, body mass index, smoking status, glucose level, heart disease condition, hypertension indicator, and stroke occurrence.

## Analysis

### Data Preparation
- **Visualization:** We examined the data using functions like `head()` and `describe()`.
- **Handling Missing Values:** We addressed missing data by replacing them with the mean or dropping them when necessary.
- **Outlier Detection:** We visualized the data for outliers, particularly in glucose levels.

### Data Exploration and Analysis
- **Correlation Matrix:** We used a correlation matrix to evaluate the relationships between attributes.
- **Assumptions:** Based on exploratory analysis, we hypothesized the impact of various factors like work type, residency, and health conditions on stroke occurrence.

### Data Pre-processing
- **Imbalanced Data Handling:** The dataset was imbalanced, with only 209 stroke occurrences. We addressed this imbalance to improve model accuracy.
- **Encoding Categorical Data:** We used `OneHotEncoder` to encode categorical variables.
- **Feature Scaling:** We applied feature scaling to ensure all variables were on the same scale.

### Machine Learning Models
We implemented various machine learning models, including Logistic Regression, Random Forest, Decision Trees, Naïve Bayes, K-Nearest Neighbors, Support Vector Machine, XGBoost, and CatBoost.

## Results and Reflections
We evaluated each model based on precision, recall, F1-score, and cross-validation accuracy. The results are summarized in the table below:

| Model       | Precision | Recall | F1-Score | Cross Validation |
|-------------|-----------|--------|----------|------------------|
| Logistic Regression | 0.77 | 0.80 | 0.78 | 78.01% |
| Random Forest       | 0.98 | 0.96 | 0.97 | 97.31% |
| Decision Trees      | 0.95 | 0.96 | 0.96 | 95.45% |
| Naïve Bayes         | 0.57 | 1.00 | 0.61 | 62.93% |
| SVM                 | 0.94 | 0.90 | 0.93 | 92.59% |
| K-NN                | 0.90 | 0.99 | 0.94 | 93.18% |
| XGBoost             | 0.99 | 0.96 | 0.97 | 97.17% |
| CatBoost            | 0.99 | 0.96 | 0.97 | 97.27% |

Our models achieved high accuracy, with XGBoost and CatBoost performing the best. The careful preprocessing, such as balancing the dataset and encoding features, contributed to these results.

## References
1. Stroke Association, “Stroke Statistics,” Stroke Association, 2020. [Link](https://www.stroke.org.uk/what-is-stroke/stroke-statistics)
2. J. M. Shikany et al., ‘‘Associations of dietary patterns and risk of sudden cardiac death in the reasons for geographic and racial differences in stroke study differ by history of coronary heart disease,’’ *Circulation*, vol. 141, no. 1, p. AP520, Mar. 2020.
3. P. B. Gorelick, “New horizons for stroke prevention: PROGRESS and HOPE,” *The Lancet Neurology*, vol. 1, no. 3, pp. 149–156, Jul. 2002.
4. "Stroke prediction through Data Science and Machine Learning Algorithms," ResearchGate. [Link](https://www.researchgate.net/publication/352261064_Stroke_prediction_through_Data_Science_and_Machine_Learning_Algorithms)
5. Kaggle, “Kaggle: Your Home for Data Science,” Kaggle.com, 2019. [Link](https://www.kaggle.com/)
6. A. Kumar, “Python - Replace Missing Values with Mean, Median & Mode,” Data Analytics, Jul. 23, 2020. [Link](https://vitalflux.com/pandas-impute-missing-values-mean-median-mode/)
7. "Missing Data: Two Big Problems with Mean Imputation," The Analysis Factor, Oct. 15, 2020. [Link](https://www.theanalysisfactor.com/mean-imputation/)
8. B. Angelov, “Working with Missing Data in Machine Learning,” Medium, Dec. 13, 2017. [Link](https://towardsdatascience.com/working-with-missing-data-in-machine-learning-9c0a430df4ce)

---

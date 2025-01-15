# Mental_Health 
Kaggle Playground Series - Season 4, Episode 11

This repository documents my work on the Kaggle Playground competition for Season 4, Episode 11. 

## Version 1: Initial Exploration

* **Objective:** Build a baseline model for predicting depression in the dataset.
* **Methodology:**
    * Dropped a significant number of columns for initial model building.
    * Implemented and compared two models: Random Forest and XGBoost.
    * Utilized GridSearchCV for hyperparameter tuning. 
* **Findings:**
    * Data analysis with Python demonstrated the ability to handle large datasets efficiently.
    * GridSearchCV yielded marginal improvements in model performance.
    * Both models achieved better-than-expected results.

## Version 2: In-depth Analysis

* **Dataset Overview:**
    * Collected from 30 cities in India.
    * Contains 234,500 rows and 18 columns.
    * Train set: 140,700 individuals with known depression diagnoses.
    * Test set: 93,800 individuals for which depression status needs to be predicted.
* **Objective:** 
    * **Data Analysis:** Investigate the influence of various external factors on depression.
    * **Model Development:** Build a predictive model to identify individuals at risk of depression.
* **Key Findings:**
    * **Students** were identified as a high-risk group for depression.
    * **City of residence** significantly influenced depression prevalence.
    * Achieved high prediction accuracy exceeding 0.92.

## Discussion

While lacking a formal psychology background, my observations align with personal experiences as a former university professor. The significant stress experienced by students concerning their future likely plays a crucial role in the development of depression. This analysis provides valuable insights into the potential impact of depression on a large scale in India, highlighting the need for targeted interventions and support programs.





## Preliminary Study of 'Students' in Depression Dataset

**Dataset Overview:**

* Total individuals: 140,700
* 'Students' category: 27,901 (less than 20% of the dataset)
* 'Students' with work: 34 individuals

**Feature Engineering:**

* **Dropped Columns:**
    * 'Name'
    * 'City'
    * 'Working Professional or Student' 
    * 'Profession'
    * 'CGPA'
    * 'Sleep Duration'
    * 'Dietary Habits'
    * 'Degree'
* **Excluded from Model:**
    * 'id' 

**Model Comparison:**

* **Objective:** Compare Random Forest and XGBoost for predicting depression.
* **Hyperparameter Tuning:**
    * Utilized GridSearchCV for both models.
    * **Random Forest:** 
        * 216 fits: Baseline accuracy 
        * 720 fits: Accuracy increased marginally (~0.1%)
    * **XGBoost:**
        * 60 fits: Baseline accuracy
        * 1280 fits: Accuracy increased marginally (~0.01%)
* **Observations:**
    * GridSearchCV offered minimal accuracy improvements for both models.
    * XGBoost demonstrated faster training times compared to Random Forest.

**Model Performance on Test Data:**

* **Random Forest (360 fits):** Score: 0.92707
* **XGBoost (540 fits):** Score: 0.93320 
* **XGBoost** achieved slightly higher accuracy.

**Key Takeaways:**

* **Computational Efficiency:** Prioritize computational efficiency by avoiding excessive hyperparameter tuning.
* **Model Selection:** Focus on selecting models that effectively maximize prediction accuracy rather than exploring numerous possibilities.
* **XGBoost** demonstrated a favorable balance between accuracy and computational efficiency in this analysis.

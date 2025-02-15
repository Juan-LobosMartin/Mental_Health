## Student/Worker Segmentation Models

This section describes the model segmentation based on student/worker status.

**Data Preprocessing:**

The following columns were processed as described:

* **Dropped Columns:**
    * `Name`
    * `Profession`
    * `CGPA`
    * `Degree`
* **Excluded from Model:**
    * `id`
    * `City`

**Model Segmentation:**

Models were segmented by `Working Professional or Student`.

**Observations:**

* Two models were trained: one for students (n=27,901) and one for working professionals (n=116,799).
* Python scripts were used for data segmentation and joining. Both Random Forest and XGBoost models were trained, with XGBoost exhibiting slightly higher accuracy (~0.000a difference).
* Initial training accuracies were 0.96179 for workers and 0.84957 for students.
* After hyperparameter tuning, training accuracies improved to 0.96183 for workers and 0.85165 for students.
* The final test data accuracy was 0.94163.

**Conclusions:**

Sample size appears to be a crucial factor for model performance.  The larger, less dispersed worker dataset yielded higher accuracy (0.96), while the smaller, more dispersed student dataset resulted in lower accuracy (0.85).

Model performance is influenced by the data distribution within each segment.  This segmentation by student/worker status proved more effective than city-based segmentation, suggesting distinct differences between these two populations.

Further investigation, potentially through additional profile questions for students, may be necessary to improve student model accuracy.

## Discussion

While lacking formal psychological training, my observations, based on personal experience as a former university professor, suggest that student stress regarding their future likely contributes significantly to depression.





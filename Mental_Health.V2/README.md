## City-Segmentation Models

This section details the city-segmentation approach used for model training.

**Data Preprocessing:**

The following columns were processed as described:

* **Dropped Columns:**
    * `Name`
    * `Profession`
    * `CGPA`
    * `Degree`
* **Excluded from Model:**
    * `id`
    * `Working Professional or Student`

**Model Segmentation:**

Models were segmented by `City`.

**Observations:**

* Model accuracy for individual cities ranged from 0.925 to 0.955.  `City_Lost` achieved an accuracy of 1.0, indicating potential overfitting (hyper-trained model).
* Python scripts facilitated the segmentation and joining of the test dataset. However, training 31 individual models required significant effort.
* For several cities, both Random Forest and XGBoost models were trained.  The performance difference between these models was minimal (on the order of thousandths).
* The final test data accuracy was 0.93464, a slight improvement over the previous version's accuracy of 0.93320.

**Conclusions:**

While differences in depression affectation exist between cities, the limited sample size (3500 to 6300 individuals per city) hindered further improvement in model accuracy.

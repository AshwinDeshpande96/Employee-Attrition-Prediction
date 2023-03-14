# Employee Attrition Prediction

* We design a ML model that creates explainable factors contributing to a employee leaving the company
* Given a list of employees that have left or still employed we predict the chances of current or future employees leaving
* Some of the information we have are as follows
    * Age
    * Travel
    * #Years of Education & the field of education
    * Commute Distance
    * Departnent
    * Income
* We perform exploratory data analysis
* Preprocessing steps to understand numeric, ordinal or categorical features and how to get them into suitable format
* Pipelining the process to ensure zero data leakage


# Feature Importance

Based of Chi2 test we find the factors influencing employee attrition

|                  **feature** | **chi2_score** |
|-----------------------------:|---------------:|
|      YearsSinceLastPromotion |     140.947662 |
|          PerformanceRating_3 |     140.181646 |
|            WorkLifeBalance_3 |     104.613632 |
|                 OverTime_Yes |     102.457300 |
|            WorkLifeBalance_1 |      96.362528 |
|               YearsAtCompany |      89.208855 |
| BusinessTravel_Travel_Rarely |      84.754307 |
|         StockOptionLevel_3.0 |      74.538308 |
|                  OverTime_No |      66.183056 |
|         MaritalStatus_Single |      64.370946 |


# Random Forest Confusion Matrix

|                 | **Predicted: No** | **Predicted: Yes** | **Total** |
|----------------:|------------------:|-------------------:|----------:|
|  **Actual: No** |               230 |                 26 |       256 |
| **Actual: Yes** |                49 |                179 |       228 |

# Random Forest Performance

|            **class** | **precision** | **recall** |   **f1** |
|---------------------:|--------------:|-----------:|---------:|
|               **No** |      0.824373 |   0.898438 | 0.859813 |
|              **Yes** |      0.873171 |   0.785088 | 0.826790 |
| **Weighted Average** |      0.847360 |   0.845041 | 0.844257 |



    

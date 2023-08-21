# Prediction-of-Product-Sale
Author: Nonlwa Mtuzula
## Data Dictionary
![image](https://github.com/NMtuzula/Prediction-of-Product-Sales/assets/138831286/034e7e07-0ee6-42b2-b4ea-ff663c25df0b)
### Exploratory Data Analysis
      - The data was first loaded using pandas and was then cleaned
      - I then visualised all categorical data to better understand the data being dealt with
![image](https://github.com/NMtuzula/Prediction-of-Product-Sales/assets/138831286/2d0e5936-b358-4a24-88ab-9945c07491f2)
#### Machine learning using the below models
      - Linear Regression Model
      - Random Forest Model
      -Tuning with GridSearchCV

##### Models Evaluated and results
  - Linear Regression Model
      Results for training data:
        - R^2 = 0.56
        - MAE = 848.383
        - MSE = 1302996.566
        - RMSE = 1141.489

      Results for testing data:
        - R^2 = 0.566
        - MAE = 807.049
        - MSE = 1198430.673
        - RMSE = 1094.729
    
 - Random Forest Model   
     Regression Metrics: Training Data
        - MAE = 299.740
        - MSE = 186,695.983
        - RMSE = 432.083
        - R^2 = 0.937
     Regression Metrics: Test Data
        - MAE = 773.526
        - MSE = 1,250,156.387
        - RMSE = 1,118.104
        - R^2 = 0.547
   
  - Tuning with GridSearchCV
     Regression Metrics: Training Data
        - MAE = 656.222
        - MSE = 875,944.722
        - RMSE = 935.919
        - R^2 = 0.704
     Regression Metrics: Test Data
        - MAE = 736.053
        - MSE = 1,122,074.080
        - RMSE = 1,059.280
        - R^2 = 0.593

###### Evaluation
Comparing Tuned data to default Random
    - Default R^2: 0.547
    -Tuned R^2: 0.593
  The training data did not improve, but there was a slight improvement on the testing data.

###### Model Recomondation
- Random Forest Model

- Justification
   - The training and test data results for this model were improving compared to the other models
  
  R-Squared, The training data had a higher chance of predicting the target value, however it did drop on the testing data but the chances were still relatively high.
  MSE- the testing data has increased drasticaly compared to the training data. Meaning it was increasing the complexity of the model by adding more features.
  The reason for selecting MSE is to show how underfitting is addressed in Machine learning.
  Using the R-Squared results for the Random Forest Model- When comparing the training and the test data, the model is overfitting.

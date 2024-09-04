# Santander Customer Satisfaction

**Importance of the problem:**

Customer satisfaction is a key measure of success. Unhappy customers do not stick around. Unhappy customers rarely voice their dissatisfaction before leaving. In order to address this problem, Santander Bank provided an anonymized dataset for identification of customer satisfaction at kaggle.com. The problem faced by the bank is that dissatisfied customers usually discontinue without prior notice. This makes it difficult for the bank to anticipate customer dissatisfaction. Lot of parameters that may influence customer satisfaction are given in the dataset and a prediction model is to be implemented in identifying the dissatisfied customers.

**Statement of Objective:**

This case study will help Santander bank in identifying dissatisfied customers early in their relationship. The solution to this problem will allow Santander to take pro-active steps when the probability of dissatisfaction of the customers increase to the point of concern, so that pro-active service approach can be adopted to avoid loss in business before it is too late.

**Dataset details:**

-	Dataset provided to this problem is anonymized and contains large number of numeric variables.
- It is a binary classification problem with a two-response variable as TARGET.
- The target column equals 1 for unsatisfied customers and 0 for satisfied customers.
- The task is to predict the probability that each customer in the test set in an unsatisfied manner.
- The performance metric that we must use here is Area under the ROC curve between the predicted probabilities and the observed target.

*Source - [Santander Customer Satisfaction](https://www.kaggle.com/competitions/santander-customer-satisfaction/data)*

**Results:**

*Results for dataset 1* <br> 
The following are the results obtained for train and CV datasets with 183 features.

| Model |Train AUC | CV AUC |
|----------|----------|----------|
| Random Forest Classifier (with 183 features)    |  0.838  | 0.810   |
| Logistic Regression (with 183 features)   |  0.802  | 0.790   |
|  K Nearest Neighbors (with 183 features)  |  0.832  | 0.796   |
| XGBoost Classifier (with 183 features)    |  0.863  | 0.840   | 
| AdaBoost Classifier (with 183 features)   |  0.847  | 0.833   |  
| Neural Networks (with 183 features)       |  0.827  | 0.823   |

*Results for  dataset 2* <br>
The following are the results obtained for train and CV datasets with top 87 features.

| Model |Train AUC | CV AUC |
|----------|----------|----------|
| Random Forest Classifier (with top 87 features)   |  0.850  | 0.815   |
| Logistic Regression (with top 87 features)   |  0.798  | 0.790   |
|  K Nearest Neighbors (with top 87 features)  |  0.833  | 0.800   |
| XGBoost Classifier (with top 87 features)    |  0.851  | 0.838   | 
| AdaBoost Classifier (with top 87 features)   |  0.830  | 0.827   |
| Neural Networks (with top 87 features)       |  0.828  | 0.821   |

- From the results for datasets 1 and 2, it is evident that XGB classifier performed better than other models.
- XG Boost Classifier performed better with top 87 features than XG Boost Classifier with 183 features.
- Here, all the models are fitted with 3-fold CV for 10 iterations.

**Kaggle Submission:**

![image](https://github.com/user-attachments/assets/52053e55-9b6a-4fe6-a54b-d7117c2a05e7)

![image](https://github.com/user-attachments/assets/7c2169ec-dac4-41a8-9951-0e933d15700a)

For more information about my case study, please feel free to go through my blog<br> 
*https://medium.com/@SharathKumarVadla/santander-customer-satisfaction-146d20d67653*

**References:**
- *https://github.com/adithyaaijth/Assessing-Classification-Methods-For-Prediction-of-Customer-Satisfaction---Santander-Bank-Dataset*
- *https://github.com/surajr/santander-customer-satisfaction/blob/master/Report.pdf*
- *https://github.com/ashishthomaschempolil/Santander-Customer-Satisfaction*




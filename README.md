# mental-health-ml
A machine learning model written using Python with the help of Jupyter notebooks.


### Objective:
Based on the given data set from the conducted survey on mental health, does a person need treatment or not?


### Motivation:
The motivation behind this question is to understand if individuals dealing with mental health challenges seek 
treatment or not. Some peple identify to have mental health challenges, but unfortunately they don't seek help or 
treatment. With this model, we can predict if the individual needs treatment or not, and use the result to better 
understand and assist individuals.


### Steps:
1. Data cleaning and transformation
2. Data visualization


### Visualizations:
1. Probability of impact on top features:
![Alt text](images/age-distribution.PNG?raw=true "Title")

2. Age distribution graph

3. Age distribution with respect to treatment

4. Cross validation accuracy

5. Most impacting features

### Train/Test Split results:
The R2 score on the training set: 0.43795214301614077

The R2 score on the testing set: 0.3718454543740196


### Cross Validation Accuracy:
CV mean accuracy score: 0.798 +/- 0.042


### Grid search accuracy:
GridSearchCV accuracy: 0.796 +/- 0.033

GridSearchCV best score:  0.7984084880636605

Best Parameter:  1.0


### Classification report:
              precision    recall  f1-score   support
           0       0.82      0.76      0.79       252
           1       0.77      0.83      0.80       251
    accuracy                           0.80       503
    macro avg      0.80      0.80      0.79       503
    weighted avg   0.80      0.80      0.79       503


### Classification accuracy using Boosting:

False Positive Rate: 0.25

Classification Accuracy:  0.8071570576540755

Classification Error:  0.19284294234592447


### Conclusion:
The top 4 features that affect whether a person should receive treatment or not is:
- Work Interference
- Family History
- Care Options
- Benefits

Age distribution is skewed toward people that are younger, so there is less data for people 
who are older than the 25-30 range.

There is chance that personal and religious beliefs might have affected this dataset, and 
resulted in some people not seek treatment despite facing challenges; thus there is a chance
for the data to be biased or not accurate.

The data set was obtained from Kaggle, and there is no information on how the data was collected.
By knowing this information, it can help us to better understand the data and the result. 


### Future Improvements:
Process the data from the comment section of the data set.

# machine-learning-challenge

Compared the various model's and the SVM model and Random Forest Model, seemed to be giving the best results among all.
And on comparing the SVM Model and Random Forest Model, the Random Forest Model gives a better accuracy and seems like the best for the Exoplanet dataset.
Saving grid2 which is of Random Forest as it has a better accuracy of .90 

## SVM Model
SVC model Train Acc: 0.846
SVC model Test Acc: 0.842
|Classification Report|
|  | precision | recall | f1-score | support |
| --- | --- |

Classification Report
                precision    recall  f1-score   support

FALSE POSITIVE       0.70      0.62      0.66       411
     CANDIDATE       0.71      0.76      0.73       484
     CONFIRMED       0.98      1.00      0.99       853

      accuracy                           0.84      1748
     macro avg       0.80      0.79      0.79      1748
  weighted avg       0.84      0.84      0.84      1748
  
#### After Parameter Tuning
{'C': 1000, 'gamma': 0.0001, 'kernel': 'linear'}
Best Score : 0.887659736791913
Test Score : 0.8890160183066361
                precision    recall  f1-score   support

FALSE POSITIVE       0.81      0.72      0.76       411
     CANDIDATE       0.79      0.84      0.81       484
     CONFIRMED       0.98      1.00      0.99       853

      accuracy                           0.89      1748
     macro avg       0.86      0.85      0.86      1748
  weighted avg       0.89      0.89      0.89      1748
  
  
## Random Forest Model
RandomForestClassifier model Train Acc: 1.000
RandomForestClassifier model Test Acc: 0.901
Feature of highest Importance is -- koi_fpflag_co
Classification Report
                precision    recall  f1-score   support

FALSE POSITIVE       0.83      0.76      0.80       411
     CANDIDATE       0.84      0.85      0.85       484
     CONFIRMED       0.96      1.00      0.98       853

      accuracy                           0.90      1748
     macro avg       0.88      0.87      0.87      1748
  weighted avg       0.90      0.90      0.90      1748
  
 #### After Parameter Tuning
{'max_depth': 175, 'n_estimators': 300}
 Best Score - 0.8933816517261111
 Test Score - 0.9038901601830663
 Classification Report
 
                precision    recall  f1-score   support

FALSE POSITIVE       0.84      0.77      0.80       411
     CANDIDATE       0.84      0.86      0.85       484
     CONFIRMED       0.97      1.00      0.98       853

      accuracy                           0.90      1748
     macro avg       0.88      0.87      0.88      1748
  weighted avg       0.90      0.90      0.90      1748



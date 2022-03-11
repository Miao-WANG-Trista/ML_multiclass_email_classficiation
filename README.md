# ML_multiclass_email_classficiation

## Data Pre-processing
In this step, we checked duplicates, wrong labels and extracted more information from 'date' and further fixed outliers.

## Feature engineering
* Normalizing numerical features
* One hot encoding for categorical features
* Feature selection
* Dimensionality Reduction

## Fix class imbalance
There are 8 classes in total however the number of their observations are not equally distributed. To avoid skewing the model training results, we tried to oversample the minority class.
## Models
We experimented with KNN, Random Forest, Catboost, SVM, Naive Bayes, XGboost as classifiers, and below are the accuracy performances.
|     Classifier     |   KNN  | Random Forest | Catboost |   SVM  | Naive Bayes | XGboost |
|:------------------:|:------:|:-------------:|:--------:|:------:|:-----------:|:-------:|
| Accuracy train set | 89.05% |     77.9%     |   87.7%  | 85.12% |    79.62%   |  89.45% |
|   Accuracy Kaggle  | 71.04% |     62.1%     |   68.0%  | 61.39% |    57.86%   |  69.14% |


During the training, we tried GridSearchCV to fine tuning the hyper parameters.


## Evaluation
We used F1-score as the metric.



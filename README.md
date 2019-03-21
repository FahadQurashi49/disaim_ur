# Urdu afsana nigar author disambiguation
## Data
Afasanas of 5 authors are being used, about 20 afsanas of each author being used
1. Devendra Satyarthi
2. Manto
3. Premchand
4. Qurratulain hyder 
5. Rajinder singh bedi
A web crawler is being used to get the the data from web:
(https://github.com/FahadQurashi49/scraper) 

## Model Used
Bi-gram model and Tri-gram model of urdu words combined
## Feature Vectors
combined Feature vecrtor of:
1. Tf-idf of words with minimum document frequecy of 20% and maximum 90% of a word
with maximum 6000 features
2. Tf-idf of Part-of-speech being used by each author in their afsanas with minimum document frequecy of 
20% and maximum 90% of a wordwith maximum 6000 features
## Proportion
75% training and 25% testing data set
## Classifier used
1. Multinomial Naive Bayes sklearn
2. SVM from sklearn
3. XGBClassifier from xgboost
## Accuracy score

|   Classifier  | Accuracy |
|:-------------:|:--------:|
| MultinomialNB |   0.56   |
|    SVM_SVC    |   0.84   |
| XGBClassifier |   0.64   |

Also see pdf attached to the project for more info on the approach used


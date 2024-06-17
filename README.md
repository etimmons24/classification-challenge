# Spam Detector

The following is a comparison of two models that classify data as either spam or no spam for an email filtering system.  The two models being compared are under the Scikit-learn API, the Logistic Regression Model (https://scikit-learn.org/stable/modules/generated/sklearn.linear_model.LogisticRegression.html#sklearn.linear_model.LogisticRegression) and a Random Forest Classifier (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html#sklearn.ensemble.RandomForestClassifier). The intention is to detemine which model is more efficient at classifying this data.  The data is sourced below and is imported using Pandas:

  * The data is located at [https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv](https://static.bc-edx.com/ai/ail-v-1-0/m13/challenge/spam-data.csv)

  * Dataset Source: [UCI Machine Learning Library](https://archive.ics.uci.edu/dataset/94/spambase)

## Initial Predictions
My first thought is that since the Logistic Regression model is specifically used for binary classification sets that it would be the best model.  There are only 
two options here, spam or no spam.  However, considering that this data set has multiple features (58) there may be better performance using the Random Forest
Classifier because of it's efficiency in preventing overfitting.

## Conclusions
The accuracy score suggests that  the RFC model performed better with an acccuracy score of 95.7% as compared to the LR accuracy score of 93%.  That 
is consistent with what I predicted.  Interestingly, the RFC model was 99.9% accurate in determining labels on training data, while the LR model was 92% accurate.

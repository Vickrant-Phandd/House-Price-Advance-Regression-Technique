# House-Price-Advance-Regression-Technique
I worked on this project because all independent features were of categorical type. To convert it into numerical values LabelEncoder and OneHotEncoding were required. Also, it is not compulsory that we have to do import sklearn all the time and do the conversion, One can manually put values without using libraries and I have done that too.

Columns like Date_of_Journey, Dep_Time, Arrival_Time, Duration is a object data type. Therefore, we have to convert this datatype into timestamp so as to use this column properly for prediction. For this we require pandas to_datetime to convert object data type to datetime dtype.

Handling Categorical Data :-
One can find many ways to handle categorical data. Some of them categorical data are,
**Nominal data** --> data are not in any order --> **OneHotEncoder** is used in this case
**Ordinal data** --> data are in order --> **LabelEncoder** is used in this case

Nominal categorical data will perform OneHotEncoding using pd.get_dummies()
Ordinal Categorical type we perform LabelEncoder Here Values are assigned with corresponding keys.

Feature Selection:-
Finding out the best feature which will contribute and have good relation with target variable. Following are some of the feature selection methods,
**heatmap**
**feature_importance_**
**SelectKBest**

Fitting model using Random Forest:-
Split dataset into train and test set in order to prediction w.r.t X_test
If needed do scaling of data
Scaling is not done in Random forest
Import model
Fit the data
Predict w.r.t X_test
In regression check RSME Score
Plot graph

Hyperparameter Tuning:-
Choose following method for hyperparameter tuning
RandomizedSearchCV --> Fast
GridSearchCV
Assign hyperparameters in form of dictionery
Fit the model
Check best paramters and best score

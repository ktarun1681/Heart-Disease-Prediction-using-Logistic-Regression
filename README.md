# Heart-Disease-Prediction-using-Logistic-Regression
Introduction

¶ WHO announced that cardiovascular diseases is the top one killer over the world. There are seventeen million people died from it every year, especially heart disease. Prevention is better than cure. If we can evaluate the risk of every patient who probably has heart disease, that is, not only patients but also everyone can do something earlier to keep illness away.  This dataset is a real data including important features of patients. This time we will build the predictable model by XGBoost library. Before predict the test dataset, use concept of crossvalid to find the optimised parameters. after that, the model can calculate the weight of each features, so we can easily understand which feature is more influent than others.  Confusion matrix is a common technique to figure out the accuracy of the model. From the standpoint of medicine, the recall rate is more important than precision rate because no one want to be misdiagnosed if the one actually have heart disease. So we will check the recall performance. After that, roc curve can help us evaluate the model, and then we'll explore the features if the model is good enough.  "Shap" is a powerful library to know whether each feature is positive or negative relationship with heart disease. At the end of the report, we double confirm the result, and we can also know which feature affect each patient the most.


Exploratory Data Analysis
There are thirteen features and one target as below:

age: The person's age in years

sex: The person's sex (1 = male, 0 = female)

cp: The chest pain experienced (Value 1: typical angina, Value 2: atypical angina, Value 3: non-anginal pain, Value 4: asymptomatic)

trestbps: The person's resting blood pressure (mm Hg on admission to the hospital)

chol: The person's cholesterol measurement in mg/dl

fbs: The person's fasting blood sugar (> 120 mg/dl, 1 = true; 0 = false)

restecg: Resting electrocardiographic measurement (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy by Estes' criteria)

thalach: The person's maximum heart rate achieved

exang: Exercise induced angina (1 = yes; 0 = no)

oldpeak: ST depression induced by exercise relative to rest

slope: the slope of the peak exercise ST segment (Value 1: upsloping, Value 2: flat, Value 3: downsloping)

ca: The number of major vessels (0-3)

thal: A blood disorder called thalassemia (3 = normal; 6 = fixed defect; 7 = reversable defect)


target: Heart disease (0 = no, 1 = yes)

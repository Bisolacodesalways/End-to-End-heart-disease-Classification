# End-to-End-heart-disease-Classification
Predicting Heart Disease using Machine Learning
This notebook looks into using various python-machine learning and data science libraries in an attempt to build a machine learning model capable of predicting whether or not someone has heart disease based on their medical attributes.

The following approach will be adopted:

1) Problem definition 2) Data 3) Sucess metrics 4) Features 5) Modelling 6) Experimentation/Evaluation

1. Problem Definition
In a case study: Given clinical parameters about a patient,can we predict whether or not they have heart disease?

2. Data
The Original data came from the cleaveland UCI repository, https://archive.ics.uci.edu/dataset/45/heart+disease. it can also be found on Kaggle.

3. Sucess metrics, what defines the sucess of the project?
If we can reach 95% accuracy at predicting whether or not a patient has heart disease during the proof of concept. We will go execute the project.

4. Features
This is where different information about each of the data features are understood or better still, employ the knowledge of a subject matter expert especially before the machine learning implementation. Understanding the data would help in order of feature importance and feature engineering-the act of encoding features(categorical) into numbers through one-hot encoding.

Create Data Dictionary

age - age in years
sex-(1 = male; 0 = female)
cp - chest pain type 0:Typical angina: chest pain related decrease blood supply to the heart 1:A typical angina: chest pain not related to heart 2:Non-anginal pain: typically esophagel spasms(non heart related) 3:Asymptomatic: chest pain not showing signs of disease
trestbps - resting blood pressure(in mmHg on admission to the hospital) anything concern
chol - serum cholestoral in mg/dl . Serum = LDL + HDL +.2* triglycerides . above 200 is cause for concern
fbs - (fasting blood sugar> 120mg/dl)(1=true;0=false) .> 126'mg/dl signals diabetes
restecg - resting electrocardiographic results .0: Nothing to note .1: ST-T Wave abnormality
 . can range from mild symptoms to severe problems
 . signals non-normal heart beat
.2.Possible or definite left ventricular hypertrophy
    .Enlarged heart;s main pumping chamber
Thalach-maximum heart rate achieved
exang- exercise induced angina(1=yes;0=no)
oldpeak-ST depression induced by exercise relative to rest
Slope- the slope of the peak exercise ST segment .0: Upsloping: better heart rate with exercise (uncommon) .1: Flatsloping: minimal change (typical healthy heart) .2: Downslopings: signs of unhealthy heart
ca- number of major vessels (0-3) colored by flourosopy . colored vessel means the doctor can see the blood passing through . the more blood movement the better (no clots)
thal- thalum stress result . 1,3: normal . 6: fixed defect: used to be detect but ok now . 7: reversible defect: no proper blood movement when exercising
target - have disease or not(1=yes, 0=no) (= the predicted attribute)

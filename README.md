# Heart-Failure-Prediction
Repo for Heart Failure Prediction Model

### Aim :
- To classify / predict whether a patient is prone to heart failure depending on multiple attributes.
- It is a **binary classification** with multiple numerical and categorical features.

### <center>Dataset Attributes</center>
    
- **Age** : age of the patient [years]
- **Sex** : sex of the patient [M: Male, F: Female]
- **ChestPainType** : chest pain type [TA: Typical Angina, ATA: Atypical Angina, NAP: Non-Anginal Pain, ASY: Asymptomatic]
- **RestingBP** : resting blood pressure [mm Hg]
- **Cholesterol** : serum cholesterol [mm/dl]
- **FastingBS** : fasting blood sugar [1: if FastingBS > 120 mg/dl, 0: otherwise]
- **RestingECG** : resting electrocardiogram results [Normal: Normal, ST: having ST-T wave abnormality (T wave inversions and/or ST elevation or depression of > 0.05 mV), LVH: showing probable or definite left ventricular hypertrophy by Estes' criteria]
- **MaxHR** : maximum heart rate achieved [Numeric value between 60 and 202]
- **ExerciseAngina** : exercise-induced angina [Y: Yes, N: No]
- **Oldpeak** : oldpeak = ST [Numeric value measured in depression]
- **ST_Slope** : the slope of the peak exercise ST segment [Up: upsloping, Flat: flat, Down: downsloping]
- **HeartDisease** : output class [1: heart disease, 0: Normal]

### Alogrithm Results Table :

|Sr. No.|ML Algorithm|Accuracy|Cross Validation Score| 
|-|-|-|-|
|1|Logistic Regression|84.78%|90.54%| 
|2|Decision Tree Classifier|82.07%|78.22%|
|3|Random Forest Classifier|85.87%|91.17%|

### Conclusion
- We have used 3 different classifiers Logistic Regression, Decision Tree and Random Forest 
- In our case, false negatives hold a high weightage. A false negative means the model incorrectly predicts that a patient does not have a disease when they actually do. In the context of heart disease diagnosis, missing a person who actually has the disease (false negatives) can have severe consequences as it may delay necessary treatment and pose a risk to the patient's health. Therefore, minimizing false negatives is crucial in this scenario.
- As we can see from the above result, Random Forest Classifier has the highest accuracy **(85.87%)** and lowest false negative rate **(8.70%)** 

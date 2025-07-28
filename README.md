
# Diabetes Risk prediction with ML and Gradio

This projects applies many supervised ML techniques to predict the probability of diabetes based on medical indicators.It uses Pima Indians Diabetes dataset and explore several preprocessing,modeling and resampling strategies.The final model is deployed using Gradio for an interative and simple to use interface.
  

## Dataset
The datasets contains medical records of female patients,including : 
- Pregnancies
- Glucose
- Blood Pressure
- Skin Thikness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age
- Outcome

## Modeling Process

**Data-Cleaning and preprocessing** : 

- Handling missing and zero-like values
- Log Transform for skewed features
- Robust and Standard scaler using ColumnTranformer

**Imbalance Handling** :
- Use of oversampling techniques such as SMOTE or ADASYN
- Use of undersampling techniques such as TomekLinks or EditedNearestNeighbors

**Model Comparison** : 
- LogisticRegression,KNN,Decision Trees,Random Forest and SVM
- Hyperparameter tuning with GridSearchCV with pipeline integration


## Gradio Web App 

The complete pipeline using the RandomForest and the oversampling technique BORDERLINESMOTE is integrated into a gradio plateform.Users can enter their medical data and received a probability of having diabetes.
- Green (Low Risk ): probability < 33%
- Orange (Moderate Risk) : 33%<=probability<=66%
- Red (High Risk) : Probability >66%

## Potential Improvement

- Feature Selection (VarianceThreshold,SelectKBest,SelectFromModel,RFECV...)
- Ensemble Methods (Voting and Stacking)
- Boosting algorithms (XGBoost,CatBoost,AdaBoost,GradientBoosting)
- Deep Neural Network to capture non-linear patterns






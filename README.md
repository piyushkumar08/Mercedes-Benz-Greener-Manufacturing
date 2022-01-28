# Mercedes-Benz-Greener-Manufacturing
Optimizing the speed of Mercedes testing system resulting in faster testing and lower carbon dioxide emissions using XGBoost

# Mercedes-Benz-Greener-Manufacturing

1. [Project Motivation](#ProjectMotivation)
2. [Installation](#installation)
3. [Data](#data)
4. [Implementation](#model)
5. [Results](#results)

## 1. Project Motivation <a name="ProjectMotivation"></a> 

- Building a model to predict the time (in seconds) that the car took to pass testing for each variable.

## 2. Installation <a name="installation"></a>

- [Jupyter Notebook](https://jupyter.org)
- Libraries :
  - pandas
  - matplotlib
  - seaborn
  - Scikit-learn
     - preprocessing (for Label_Encoder)
     - decomposition (for PCA)
     - model_selection (for train-test-split and GridSearchCV)
     - metrics ( for rmse) 
  - xgboost
 
## 3. Data<a name="data"></a> 
- [Datasets](https://github.com/piyushkumar08/Mercedes-Benz-Greener-Manufacturing/tree/main/Datasets) is related to testing time for each variable like suspension, airbags, etc having 4209 records each for training and testing datasets. 
- Attribute information:
    -  ‘y’ represents the time (in seconds) that the car took to pass testing for each variable
    -  Other 376 variables represent a custom feature in a Mercedes car

## 4. Implementation <a name="model"></a> 
- Preprocessing for both train and test data:
    - removal of features having zero variability
    - null value treatment
    - Label encoding for categorical columns
    - Dimensionality reduction using PCA 
- Extraction of Dependent and Independent variables 
- Applying Crossvalidation technique to get training and testing data 
- Modelling on training data using XGboost 
- Hyperparamter tuning is also done using GridSearchCV from sklearn to get the best accuracy and optimal parameters for training the model
- Prediction is done on Test dataset.      

## 5. Result<a name="results"></a>
- The details of the results - [Mercedes.ipynb](https://github.com/piyushkumar08/Mercedes-Benz-Greener-Manufacturing/blob/main/Mercedes.ipynb)

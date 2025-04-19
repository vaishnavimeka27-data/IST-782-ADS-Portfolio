# Predictive Modeling of Diabetes Health Indicators


## Team members
**Hang Tian**(the point of contact)\
github id:ht6631

Mengqi Li\
github id:Adalmqqqq

Vaishnavi Meka\
github id:vaishnavimeka27


## Introduction
In this project, our goal is to create a model that can predict an individual's likelihood of developing diabetes using classification machine learning algorithms. By analyzing data on eating habits, lifestyle habits and past medical history, we intend to find out which factors are most likely to lead to diabetes. Our objective is clear: use data collected by the CDC on a variety of health indicators to accurately identify people at high risk for diabetes and to make this information available to everyone, regardless of their medical knowledge.\
\
We use a comprehensive dataset that integrates a wide range of health indicators, including not only traditional indicators such as blood glucose levels and body mass index, but also lifestyle factors, socioeconomic status, environmental influences and genetic predisposition. In addition, our predictive models are designed to provide more accurate predictions based on different individual health conditions. \
\
The stakeholders in our project are diverse. Potential stakeholders include people who are at high risk of developing diabetes and related medical institutions. Through our trained model, we can not only help healthcare professionals identify at-risk patients early and provide targeted advice and treatment to prevent progression, but the model itself can also explain which features have a greater impact on a patient's likelihood of developing diabetes, potentially preventing it before it occurs. Moreover, policymakers and public health officials can use our modeling results to develop more effective diabetes prevention and management programs.


## Literature Review
The condition known today as diabetes may be recorded tracing back to 1550 BC on the Ebers Papyrus[^1]. Having harmful effects on human body[^2], it is long been studied by various scholars on its mechanism from centuries ago[^3]. Recent years have seen many studies combining machine learning algorithms and diabetes prediction[^4],[^5],[^6]. Among these studies, typical classification algorithms such as decision trees, k-nearest neighbor, support vector machines are tested to perform acceptable for diabetes prediction, as well as boosting and bagging alrgorithms like XGBoost, AdaBoost and random forest. However, these studies only included limited features[^4],[^5] or suffered from the lack of observations on their selected dataset[^6].\
\
On the contrary, thanks to the diligent work of the CDC, we are provided with a data set with sufficient amount of observations and features. In this project, we will leverage the abundant amount of records and work on feature engineering to train a best classification model for diabetes prediction.


## Data and Methods
### Data
Link to the Data: https://archive.ics.uci.edu/dataset/891/cdc+diabetes+health+indicators

#### Summary Information
The original dataset has 21 categorical and numeric features with 253,680 observations\
\
Features likely include numerical data (e.g., age, BMI), binary data (e.g., presence or absence of diabetes).

#### Data's provenance
It comes from the “CDC Diabetes Health Indicators” dataset collected in the UCI machine learning repository. It is a survey response to the CDC's BRFSS2015.\
\
For this project we plan to select only some of these features for classification through feature engineering.


### Methods
#### Modeling Approach
Data Preprocessing: Necessary steps: handling missing values, encoding categorical variables, normalizing and scaling numerical features and dealing with unbalanced data.
Feature Selection: Correlation analysis, identify the most relevant features for diabetes prediction.
#### Modeling Techniques
Consider a range of machine learning models, from logistic regression to more complex models like random forests, gradient boosting machines.
##### Model Evaluation
For our project models, accuracy, sensitivity (recall), specificity are critical metrics.

#### Model Validation
Employ cross-validation techniques to ensure the model's generalizability. Consider using stratified folds if the dataset is imbalanced to maintain the proportion of the target variable across each fold.


## Project Plan
Period|Activity|Milestone
|---|---|---|
|3/4 - 3/18|EDA </br> Data cleaning and preprocessing </br> Initial feature selection </br> Establish base models|Data exploration was completed, the dataset cleaned and preprocessed, and candidate approaches for modeling were finalized.
|3/18 - 4/1|Advanced feature engineering </br> Develop complex models </br> Begin model validation and tuning|Advanced features were developed, complex models trained, and initial model validation and tuning completed.
|4/1 - 4/15|Finalize model tuning </br> Complete model validation </br> Draft report|Optimized models are ready for evaluation, and validation results have been thoroughly documented.
|4/15 - 5/1|Finalize report writing </br> Prepare presentation and submission| Final report finalized and proofread, Presentation ready for delivery.


## Risks
1. A larger data set means higher amount of rare conditions (e.g. people should be identified as under high-risk but don’t have diabetes). This may cause lower accuracy or recall rate of our model.
2. Among the 250 thousand observations, only about 30 thousand people have diabetes. Our dataset is biased. This asks us to use multiple metrics to measure a meaningful prediction accuracy.
3. Due to the large number of features, it is possible for the model to learn noise and details from the training data that do not generalize well to unseen data. This requires us to regularize the model, use cross-validation, and possibly reduce the feature space through selection techniques or dimensionality reduction.



## References
[^1]: History of diabetes on Wikipedia (https://en.wikipedia.org/wiki/History_of_diabetes)
[^2]: Vaishali, R., et al. "Genetic algorithm based feature selection and MOE Fuzzy classification algorithm on Pima Indians Diabetes dataset." 2017 international conference on computing networking and informatics (ICCNI). IEEE, 2017.
[^3]: Karamanou M, Protogerou A, Tsoucalas G, Androutsos G, Poulakou-Rebelakou E. Milestones in the history of diabetes mellitus: The main contributors. World J Diabetes. 2016 Jan 10;7(1):1-7. doi: 10.4239/wjd.v7.i1.1.
[^4]: J. Pradeep Kandhasamy, S. Balamurali, Performance Analysis of Classifier Models to Predict Diabetes Mellitus, Procedia Computer Science, Volume 47, 2015, Pages 45-51, ISSN 1877-0509, https://doi.org/10.1016/j.procs.2015.03.182.
[^5]: Sisodia, Deepti, and Dilip Singh Sisodia. "Prediction of diabetes using classification algorithms." Procedia computer science 132 (2018): 1578-1585.
[^6]: M. K. Hasan, M. A. Alam, D. Das, E. Hossain and M. Hasan, "Diabetes Prediction Using Ensembling of Different Machine Learning Classifiers," in IEEE Access, vol. 8, pp. 76516-76531, 2020, doi: 10.1109/ACCESS.2020.2989857.

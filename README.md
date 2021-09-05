
# University Admission Prediction deployed on cloud services
## Objective
To find the chance of admit of a candidate based on GRE Score, TOEFL Score, University Rating, SOP Score, LOR Score, CGPA and Research Experience.

The model takes in GRE Score, TOEFL Score, University Rating, SOP Score, LOR Score and CGPA as inputs to predict the probability of a candidate getting university admission on percentage basis. 


## Data
[Dataset](https://github.com/MarurSrikanta/LinearRegression-Deployment/tree/main/Data) is available on Kaggle and the features are as below

**GRE Score:** float64, maximum value of 340

**TOEFL Score:** float64, maximum value of 120

**University Rating:** float64, maximum value of 5

**SOP:** float64, maximum value of 5

**LOR:** float64, maximum value of 5

**CGPA:** float64, maximum value of 10

**Research:** int64, takes values 0 or 1, 0 for no research experience and 1 when candidate has research experience

**Chance of Admit:** float64, the predicted variable which gives the chance of candidate getting admitted into a university in percentage



## Application Design
Once the data source is fixed, the approach consists of two pipelines:
a) **Training Pipeline** which includes data preprocessing, selecting the right algorithm for creating machine learning model, checking accuracy of model and saving the model

![alt text](https://github.com/MarurSrikanta/LinearRegression-Deployment/blob/main/Images/Training_Pipeline.png)


b) **Testing Pipeline** where the trained model is exposed as an API for user consumption. For prediction, the saved model is first loaded and predictions are made. The web app is deployed to cloud platform.

![alt text](https://github.com/MarurSrikanta/LinearRegression-Deployment/blob/main/Images/Testing_Pipeline.png)

## Deployment links
The model is deployed in three cloud services.

[AWS](http://linearregressiondeploy-env.eba-9jdrquhj.eu-west-1.elasticbeanstalk.com)

[Azure](https://linearregression-deploy.azurewebsites.net)

[Heroku](https://linearregression-deploy.herokuapp.com)

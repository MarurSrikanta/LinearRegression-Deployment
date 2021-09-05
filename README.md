
# Linear Regression Model for university admission prediction deployed on AWS, Azure and Heroku.

## Objective
To find the chance of admit of a candidate based on GRE Score, TOEFL Score, University Rating, SOP Score, LOR Score, CGPA and Research Experience.

The model takes in GRE Score, TOEFL Score, University Rating, SOP Score, LOR Score and CGPA as inputs to predict the probability of a candidate getting university admission on percentage basis. 


## Data
Data is available on Kaggle

[Dataset](https://github.com/MarurSrikanta/LinearRegression-Deployment/tree/main/Data)



## Application Design
Once the data source is fixed, the approach consists of two pipelines:
a) **Training Pipeline** which includes data preprocessing, selecting the right algorithm for creating machine learning model, checking accuracy of model and saving the model

![alt text](https://github.com/MarurSrikanta/LinearRegression-Deployment/blob/main/Images/Training_Pipeline.png)


b) **Testing Pipeline** where the trained model is exposed as an API for user consumption. For prediction, the saved model is first loaded and predictions are made. The web app is deployed to cloud platform.

![alt text](https://github.com/MarurSrikanta/LinearRegression-Deployment/blob/main/Images/Testing_Pipeline.png)

**Deployment links are below:**

[AWS](http://linearregressiondeploy-env.eba-9jdrquhj.eu-west-1.elasticbeanstalk.com)

[Azure](https://linearregression-deploy.azurewebsites.net)

[Heroku](https://linearregression-deploy.herokuapp.com)

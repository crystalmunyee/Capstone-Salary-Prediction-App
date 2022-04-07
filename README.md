# Capstone-Salary-Prediction-App

## Introduction:
- There has always been a gap of the salary expected form both job seekers and hiring organizations. 
- This usually because candidates are not able to gauge their true value in the market.
- This project aims to bridge the gap for both parties by developing a model to learn the salary expectations from the kaggle dataset collected in UK.

## Problem Statement:
1. Identify salary ranges for a certain position in Data Science job postings
2. Investigate the best model for salary prediction based on job description.
3. The Model performance will be evaluated by the MSE, MAE and the accuracy for classification problem.
4. Find out top skill or traits potential employers are looking for.
5. Deploy an app for job seekers to determine current market salary rates based on their job skills.

## EDA
### Job sector vs Salary:

![image](https://user-images.githubusercontent.com/88234945/162124782-3e32fc18-e06e-4a9d-b509-6c50bd4f9df3.png)

Theres quite an interesting find on the salary averages in different sectors.

## Executive Summary:
![image](https://user-images.githubusercontent.com/88234945/162124431-abab8404-217e-4270-95d1-fa42a9c05d93.png)

From the modelling summary table, we can deduce that Extra Tree Classifier is the most suitable model for this application compared to the rest in terms of MSE, MAE and accuracy. It also performs better than our baseline model which is expected to be ~35% only for accuracy.

![image](https://user-images.githubusercontent.com/88234945/162125455-fd99f2ee-2fa0-443b-babc-c8cc08e48535.png)

Looking into the models top features, we can say that applicants can focus on these key qualities to help improve their resume and also position them in a better place.

## Conclusion:
As a conclusion, we will be using the Extra Trees Classifier on the final model to predict salary for the web app. We found that the job description NLP classification works best. So we had to drop the other features such as location even though EDA shows some correlation but the model accuracy drops significantly when we ran it  together using pycaret.

## Recommendation:
- The trend might change with recent job requirement shift and new industries popping up from time to time. It serves as a caveat that this model is not robust to predict all future changes. So, future studies its best to update the model with new data.
- The web app is useful for predficting salary but I think future works can be done to also include recommendation systems for certain users.

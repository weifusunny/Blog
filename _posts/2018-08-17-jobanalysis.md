---
layout: post
title: Data science positions analysis
---

This project is about web scraping, EDA and machine learning algorithm implementations.

In the first stage of the project, I have scraped 1394 jobs advertised on www.seek.com.au. Every record of every scraped job posted on the website contains the job title, job description, the salary where applicable, the company location and the industry to which each company belongs.
I have scraped the entire data in five separate categories:
1. Data Scientist
2. Data Analyst
3. Data Engineer
4. Business Intelligence Developer
5. Data Science Consultant

The scraped data has been saved in five separate .csv files, corresponding to the five categories above.

In the second stage of the project, I have cleaned the data by removing nulls and extracting the salary ranges listed in the salary columns. Among the 1394 advertised jobs, I have managed to obtain 380 valid salary values.

In the third stage of the project, I have done EDAs to display the average salary for each location, for each industry, for each category, in the form of bar charts. I have also displayed the salary distribution as a histogram.The EDAs show that the salaries do not vary significantly between different locations and between different industries. Instead the variation is caused by the category and the professional level of the position. Based on this we can conclude that the salary correlates to the job title and the job category.

In the fourth stage of the project, i used TDIDFvectoriser of Nature Language Processing( NLP) to determine the relevent features for predicting salary. I have used two machine learning algorithms to train a known salary dataset and predict the salary for the test dataset. One machine learning algoritm is the multiple linear regression with Ridge regularisation. The second machine learning algorithm is the decision tree regression. The comparison between the two algorithms shows that they have yielded very similar prediction results, both for the training and the test data.

In the fifth stage of the project, I have used the countvectoriser of NLP to analyse and extract more than 2000 features from all job descriptions use the extracted features to fit and transform the job description dataset. Based on the fitted dataset i have identified the key words for the positions of each category. Following that I have used the KNN and ensemble bagging KNN to feed the dataset with more than 2000 features and the ensemble bagging KNN has achieved a better score.

Thank you for reading. More details refer to my github: github.com/weifusunny/jobanalysis.


---
layout: post
title: Data science positions analysis
---

This project is about web scraping of, EDA and machine learning algorithm implementations on the data of data science related positions.

In the first stage of the project, I have scraped 1394 jobs advertised on www.seek.com.au across the whole Australia within the recent two months. Every record of every scraped job posted on the website contains the job title, job description, the salary where applicable, the company location and the industry to which each company belongs.
I have scraped the entire data in five separate categories:
1. Data Scientist
2. Data Analyst
3. Data Engineer
4. Business Intelligence Developer
5. Data Science Consultant

The scraped data has been saved in five separate .csv files, corresponding to the five categories above.

In the second stage of the project, I have cleaned the data by removing nulls and extracting the salary ranges listed in the salary columns. Salary column is the most interesting part. Here are some examples:

       '$120,000 - $159,999', '$100k - $150k p.a.',
       'Base + Super + Profit Share',
       '£110000.00 - £130000.00 p.a. + super and bonus',
       'Highly competitive package', 'Base + Super + Bonus',
       'Up to $190,000 + super + 20% bonus',
       '$40,000 - $49,999', '$400 - $500 p.d. + Super', '$85k Package'
       'US$100k - US$130k p.a.',

We can see that the salary may be specified as a number per hour, per day, per annum, p.a., p.d., with or without $, in US$ or in pound, with or without 'k', single number or a range. Anyway, a user-defined function is written with Regex applied in the number extracting. Finally among the 1394 advertised jobs, I have managed to obtain 380 valid salary values which are the annual income numbers.

In the third stage of the project, I have done EDAs to display the average salary for each location, for each industry, for each category, in the form of bar charts. I have also displayed the salary distribution as a histogram.The EDAs show that the salaries do not vary significantly between different locations and between different industries. Instead the variation is caused by the category and the professional level of the position. Based on this we can conclude that the salary correlates to the job title and the job category.

Here are some interesting numbers:

1. 710 positions are based in Sydney and 366 in Melbourne, much less in other cities or areas

2. 809 positions are in the industry "Information &  Communication technoloy" and 105 in "Science & Technoloy", much fewer in other industries

3. The highest average salary is in Perth and in "Legal" industry, however, due to small number of samples this information might be misleading

4. The middle 50% of the salaries range between 100k and 160k. A few outliers are above 230k. The most frequent salary is around 100k. The salary distribution does not follow normal distribution pattern.

In the fourth stage of the project, i used TDIDFvectoriser of Nature Language Processing( NLP) to determine the relevent features for predicting salary. I have used two machine learning algorithms to train a known salary dataset and predict the salary for the test dataset. One machine learning algoritm is the multiple linear regression with Ridge regularisation. The second machine learning algorithm is the decision tree regression. The comparison between the two algorithms shows that they have yielded very similar prediction results, both for the training and the test data.

In the fifth stage of the project, I have used the countvectoriser of NLP to analyse and extract more than 2000 features from all job descriptions use the extracted features to fit and transform the job description dataset. Based on the fitted dataset i have identified the key words for the positions of each category. Following that I have used the KNN and ensemble bagging KNN to feed the dataset with more than 2000 features and the ensemble bagging KNN has achieved a better score.

For a role of 'data scientist', these key words in job descriptions differentiate ths position (the importance level is denoted as a number next to it):

    data           0.989130    
    scientist      0.282609    
    analytics      0.244565    
    join           0.211957    
    team           0.211957    
    looking        0.173913    
    opportunity    0.173913    
    science        0.141304    
    business       0.141304    
    role           0.135870
    
Here are the results for a role of 'business intelligence developer':

    business        0.308989    
    developer       0.230337    
    bi              0.207865    
    data            0.207865    
    team            0.196629    
    intelligence    0.196629    
    join            0.185393    
    opportunity     0.174157    
    looking         0.151685    
    work            0.146067

In summary, this is a very interesting and challenging project. After completing this, I have practised and mastered a lot of skills: data scraping, data cleaning, Regex, KNN, decision tree, linear regression, ensemble, NLP and so on.

Thank you for reading. More details refer to my github: github.com/weifusunny/jobanalysis.


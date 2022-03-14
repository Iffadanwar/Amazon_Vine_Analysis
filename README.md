# Amazon_Vine_Analysis

## Background
Since your work with Jennifer on the SellBy project was so successful, you’ve been tasked with another, larger project: analyzing Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies like SellBy pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

In this project, you’ll have access to approximately 50 datasets. Each one contains reviews of a specific product, from clothing apparel to wireless products. You’ll need to pick one of these datasets and use PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, you’ll use PySpark, Pandas, or SQL to determine if there is any bias toward favorable reviews from Vine members in your dataset. Then, you’ll write a summary of the analysis for Jennifer to submit to the SellBy stakeholders.

## What You're Creating
This new assignment consists of two technical analysis deliverables and a written report. You will submit the following:

Deliverable 1: Perform ETL on Amazon Product Reviews
Deliverable 2: Determine Bias of Vine Reviews
Deliverable 3: A Written Report on the Analysis (README.md)

## Analysis Overview
The goal of this analysis is to better understand if Amazon's Vine membrers write more favorable reviews on their product.
The analysis uses PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, load the transformed data into pgAdmin and calculate different metrics.
We focused on the US reviews for Mobile electronic items. Amazon is a comon place to shop for mobile phone and assessories which is why I chose this data set.

## Resources
- Data Source: Amazon Review datasets, Video Games Review dataset
- Software: Google Colab Notebook, PostgreSQL 11.9, pgAdmin 4, AWS

Data from Amazoon cloud data base was successfully uploaded to post gress.

![diliv 1.1](https://github.com/Iffadanwar/Amazon_Vine_Analysis/blob/main/images/diliv_1.1.png)

## Results
After Analysis of the vine comments the following results were evaluated.

![diliv 2.1](https://github.com/Iffadanwar/Amazon_Vine_Analysis/blob/main/images/diliv_2.1.png)

total paid reviews from vine = 4
total paid reviews and that gave a 5 star = 1
percent of 5 star and paid review = 25%

![diliv 2.2](https://github.com/Iffadanwar/Amazon_Vine_Analysis/blob/main/images/diliv_2.2.png)

total paid reviews from vine = 1064
total paid reviews and that gave a 5 star = 527
percent of 5 star and paid review = 49.53%

## Summary
- The problem derived from this dataset is thats the number of paid vine reviwes are extremely low, only 4. This gave a percent 5star review of only 25%
- ~50% of non paid users gave the app 5 stars showing that there is no positivity bias for reviews in the Vine program.
- I would additionally look at more databases to see how other product types fair.
- Additionally we could analyse the statistical distribution (mean, median and mode) of the star rating for the Vine and non-Vine reviews.


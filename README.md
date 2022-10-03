# Amazon_Vine_Analysis

## Overview of the analysis
The purpose of this analysis is to analyze Amazon reviews written by members of the paid Amazon Vine program. The Amazon Vine program is a service that allows manufacturers and publishers to receive reviews for their products. Companies pay a small fee to Amazon and provide products to Amazon Vine members, who are then required to publish a review.

Amazon publishes approximately 50 [Amazon Review datasets](https://s3.amazonaws.com/amazon-reviews-pds/tsv/index.txt). Each one contains reviews of a specific product, from clothing apparel to wireless products. In my analysis, I have picked the Outdoors datasets and used PySpark to perform the ETL process to extract the dataset, transform the data, connect to an AWS RDS instance, and load the transformed data into pgAdmin. Next, I have used PySpark to determine if there is any bias toward favorable reviews from Vine members in the Outdoors dataset. In my summary, I state if there is any positivity bias for reviews in the Vine program.

## Results
The following bullets summarize the outcome of my analysis for the Outdoors dataset:

- Total number of reviews:  2302401
- Number of 5 star reviews:  1434884
- Number of Vine reviews:  107
- Number of 5 star Vine reviews:  56
- Percentage of 5 star Vine reviews:  52.336448598130836
- Number of non-Vine reviews:  39869
- Number of non-Vine 5 star reviews:  21005
- Percentage of 5 star non-Vine reviews:  52.68504351751988



## Summary
Based on the results from my analysis, I don't see a bias for reviews in the Vine program. The percentage of 5 star reviews from members of the Vine program is 52.3% and the percentage of 5 star reviews from non-members is 52.7%.  

 One additional analysis that I could do with the dataset to support my statement is to analyze if reviews by Vine members are considered more helpful than reviews by non-members by looking at the data provided in the column helpful_votes. 


# Amazon_Vine_Analysis

### Overview:
For this project, we are analyzing Amazon reviews written by members of the paid Amazon Vine program. 
First I used PySpark to extract and transform the data. Then I connected to an AWS RDS instance and loaded the transformed data into pgAdmin.
I again used PySpark to filter the data to determine if there is bias toward favorable reviews among the paid members in the Vine program.

### Results: 

- I reviewed a total of 45,421 reviews. These were filtered from the whole to dataset to include only reviews that contained more than 
20 total votes and over 50% helpful votes.
- There were 23,748 5 star reveiws.
- 52% of all reviews were 5 star.


![vine_reviews](https://github.com/lindseyasterman/Amazon_Vine_Analysis/blob/main/vine_reviews.png)
- There were 33 total paid reviews. 
- 15 of those were 5 stars.
- 45% of paid reviews were 5 star.


![nonvine_reviews](https://github.com/lindseyasterman/Amazon_Vine_Analysis/blob/main/nonvine_reviews.png)
- There were 45,388 total un-paid reviews.
- 23,733 of those were 5 stars.
- 52% of un-paid reviews were 5 stars.


### Summary: 
There does not appear to be a positivity bias for reviews in the Vine program. In fact, paid reviews showed a lower percentage of 
5 star ratings. To further study the data, we could filter the data for verified purchases. This would help to remove possible fraudulent reviews.
This data set contained very few reviews from the vine program. It would be important to perform this same process 
on another dataset to see if the results are the same with a larger sample to study. 

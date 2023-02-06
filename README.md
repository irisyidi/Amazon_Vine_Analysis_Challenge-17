# Amazon_Vine_Analysis_Challenge-17

## Overview of the analysis

The purpose of the analysis is to provide insights from the reveiws written by members of the paid Amazon vine Program. From the watch dataset selected (https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Watches_v1_00.tsv.gz), ETL process is performed by PySpark and the cleaned data is loaded to pgAdmin. Then through Pandas, the bias towards favorable reviews from Vine members in the dataset is determined. 

## Results

Below are the screenshots of codes to perform the required calculation of reviews and related percentages. 

![Deli3-1](https://github.com/irisyidi/Amazon_Vine_Analysis_Challenge-17/blob/main/Deli3-1.png)

![Deli3-2.png](https://github.com/irisyidi/Amazon_Vine_Analysis_Challenge-17/blob/main/Deli3-2.png)


- How many Vine reviews and non-Vine reviews were there?

From the vine table extracted from database, the total number of Vine reviews are 1,747 and the total number of non-Vine reviews are 959,125. 

- How many Vine reviews were 5 stars? How many non-Vine reviews were 5 stars?

Among 1,747 Vine review, the five star Vine reviews are 605. Among the non-Vine reviews, 571,022 non-Vine reviews are five stars. 

- What percentage of Vine reviews were 5 stars? What percentage of non-Vine reviews were 5 stars?

 0.35 of Vine reviews were five stars. 0.60 of non-Vine reviews were five stars. 


## Summary

### Conclusion

From the results show above, there is obvious bias between the reviews in the Vine program and the review not in the Vine program. the percentage of 5 stars  from Vine program is lower than that from non_Vine program. Therefore, Vine members are more likely not to give favorable reviews than non-Vine members. 

### Additional analysises

We can make analysis of the number and the percentage of reviews from the Vine and non-Vine members in the total five star reviews.

Besides, line chart the rating of both Vine members and non-Vine members can be depicted  by using the review stars as x-axis and the number of reviews as y-axis. 

# Amazon_Vine_Analysis

Analysis on Amazon's vine review program using PySpark and AWS RDS with PostgreSQL

**Overview**

In this project I used US Apparel product reviews from Amazon. The goal was to analyze if it would be worth it to subscribe to a Vine program if we were to sell similar products through their platform. The vine review program is an incentive model in which customers are gifted free stuff when they write good reviews. I was able to use PySpark to extract, transform, and load (ETL) the data to a AWS RDS I created and connected to my PostgreSQL server to be able to query it and extract my finished tables from there. Part of the data transformation was made using pandas as well.

The objective of this project was to familiarize myself with Spark. Apache Spark is a unified analytics engine for large-sacale data processing. This means that when working with big data, Spark is one of the best technologies out there to use because of its in-memory computation instead of disk-based solution. It allows for lazy evaluation and delaying expressions or commands until its needed.

**Resources**

  Datasets:- US Apparel dataset

**Technologies Used**

  Google Colab (to run PySpark),
  Jupyter Notebook,
  AWS S3 and RDS,
  PostgreSQL
  
 **Data Frames:**
  ![image](https://user-images.githubusercontent.com/96051648/163248492-acd64cf5-60e0-4002-8e9a-74cfcebf2409.png)
  
  ![image](https://user-images.githubusercontent.com/96051648/163248625-d1a1e178-3734-4c16-b168-98c6b78a01f6.png)

  ![image](https://user-images.githubusercontent.com/96051648/163248705-84ef7af2-ad6a-4ff5-b577-23b629030a3f.png)

  ![image](https://user-images.githubusercontent.com/96051648/163248802-4ba4e281-1a52-4271-844f-cec6bdfa3893.png)


**Summary**

In conclusion, the vine program might just not be worth it for the apparel category. As it can be seen, there were not many helpful reviews that made part of it (total of 33), and only around half of them were 5-star rated (45%). 

Very similarly to the unpaid reviews which also only half of them were 5 star rated (52%). Even though the percentages may be misleading as the volume of reviews in the vine and non-vine programs vary so much, this itself is a sign that the vine program is not very popular in this category. We might not want to pay for it as it is not incentivizing the people to write better reviews.

Paid Vine Program

- 33 total reviews
- 15 5-star reviews
- 45.5% of vine reviews were 5-star

Unpaid reviews

- 45,388 total reviews
- 23,733 5-star reviews
- 52.3% of unpaid reviews were 5-star

This allows us to conclude that customers don't feel a positivity bias for leaving good reviews in the paid program as there are so few and not so many well-rated. Nevertheless, if we were to further analyze we could calculate the mean of the star ratings on each programs' reviews to see if there's a significant incentive.

A recommendation would be to apply a NLP sentiment analysis to check for the words used in the majority of the reviews. This way we could see if vine reviews are more touching and detailed, that we can feel customers have an incentive to leave great reviews.

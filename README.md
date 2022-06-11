# Amazon_Vine_Analysis
## Overview 
The purpose of this project is to analyze Amazon Vine Program, in which trusted reviewers are invited and paid for posting reviews about certain products. The point is to determine if there is any bias to positive reviews from those paid reviewers. We are going to apply the ETL process to download the data of an AWS database, then we will analyze the data to determine if there's a bias or not. 

## Resources
AWS, Spark, pgAdmin, Google Colaborate, and database from url = "https://s3.amazonaws.com/amazon-reviews-pds/tsv/amazon_reviews_us_Personal_Care_Appliances_v1_00.tsv.gz"

## Results
First in *Amazon_Reviews_ETL.ipynb* the we used Spark to extract the data, then it was transform into the next 4 DataFrames and loaded them to fill the tables in pgAdmin.

![Screen Shot 2022-06-11 at 12 08 03 PM](https://user-images.githubusercontent.com/43548929/173201644-5ac74940-94a9-45e9-a4e4-018dee6fad08.png)

![Screen Shot 2022-06-11 at 12 08 22 PM](https://user-images.githubusercontent.com/43548929/173201649-71fa2eaa-1b89-4246-b3bf-a105571d6a2b.png)

![Screen Shot 2022-06-11 at 12 08 34 PM](https://user-images.githubusercontent.com/43548929/173201656-169c17b5-d81d-4838-ae55-063dd90711e5.png)

![Screen Shot 2022-06-11 at 12 08 51 PM](https://user-images.githubusercontent.com/43548929/173201665-8bd2fa3c-3a1d-4bc5-a2ae-f9cc61bd8b54.png)

Then using pySpark on the dataFrame *vine_table* we filtered the data and got these results:

**Total number of reviewers, vine-reviwers and no vine-reviewrs**

![Screen Shot 2022-06-11 at 12 34 55 PM](https://user-images.githubusercontent.com/43548929/173202348-624ed314-fa92-460b-81e5-10fdfa762cc9.png)

**Total 5-star reviews from vine-reviewrs and no vine_reviewr**

![Screen Shot 2022-06-11 at 12 38 19 PM](https://user-images.githubusercontent.com/43548929/173202433-933468f8-e89c-42c4-bd86-ac0085de2148.png)

**Percentage of 5 star reviews**

![Screen Shot 2022-06-11 at 12 38 43 PM](https://user-images.githubusercontent.com/43548929/173202443-cdf38f5f-e4bd-46c0-8426-bba5026ac5fc.png)


## Summary


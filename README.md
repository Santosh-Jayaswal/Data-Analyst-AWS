# Data-Analyst-AWS

This document is about analyzing the Vancouver Trees Dataset, which shows the number of trees of specific species planted on different streets in Vancouver (Street Trees, 2024). For this analysis, we will use AWS Cloud Platform considering data analytics tools such as Glue, Data Brew, and S3 to process the data. First, we will load the raw data into S3 (ingestion). Then, we will clean and profile the data using Data Brew to remove any missing values, duplicates, or unnecessary columns, ensuring the data is ready for analysis. Finally, we will design an ETL pipeline using AWS Glue to transform and extract actionable insights. The following image illustrates the operational workflow: 

![street-trees-drawio](https://github.com/user-attachments/assets/cb4705d8-e72f-4311-ba7f-99a2da9284cc)

# Descriptive Analytics
1. **Project Description**: Identifying the most frequent street for tree planting to plan maintenance and future planting strategies.
2. **Project Title**: Highlighting popular street having trees.
3. **Objective**: This data can help the city prioritize streets with greater capacity for trees get sufficient attention for maintenance such as watering, pruning, pest control while promoting environmental equity.
4. **Dataset**: This dataset has certain attributes that describe.

    •	TREE_ID: A unique ID for each tree.

    •	STD_STREET: The name of the street where the tree is located.

    •	SPECIES_NAME: The type of tree.

    •	NEIGHBOURHOOD_NAME: The local area in Vancouver where the tree is found.

5.    **Methodology**:

      i.    **Data Collection and Preparation**: After downloading the CSV data, we moved raw file into _raw_ directory under AWS S3 bucket in order to perform
      cleaning and transforming process with the help AWS DataBrew. We removed null values, duplicates to maintain consistencies in the data. And then moved cleaned
      data back into S3 _transform_ directory in S3 bucket.
  
      ii.    **Data Wrangling**: Next, we are going to fetch schema of data using AWS Glue Crawler to make the operation seamless for further analytics.
  
      iii.    **Data Analysing**: We have used AWS Athena to write SQL Query for extracting insights.![Picture2](https://github.com/user-attachments/assets/f383e04b-d4f0-4f1d-8135-9611e64e64fe)

      iv.    **Insights and Findings**: Streets like Macdonald and Alberta are identified as the most popular locations of the Vancouver where municipality need to 
      focus a maintain fostering enviornment equity.

      v.    **Data Encryption**: Its important to keep data secure and KMS is a best service which provide a key using it we can protect our S3 bucket from hackers or 
      breaching.

      vi.    **Monitoring and Controlling Operation**: AWS has variety of services to serve particular perpose. For this, we have used CloudWatch service to create 
      dashboard where we contineously monitor the cost, bucket size, and logs of error of ETL job.![Picture1](https://github.com/user-attachments/assets/0612bec7-263a-45e5-bc65-712158b40847)


7.    **Tool and Technology**: In this project we have only used AWS Cloud Services, S3 for storing and retrieving data, Glue and Data Brew for ETL job, Athena to extracting business insights, KMS for encrypting data, and CloudWatch for monitoring and controling to make operation smooth and secure.

# Data-Analyst-AWS

This document is about analyzing the Vancouver Trees Dataset, which shows the number of trees of specific species planted on different streets in Vancouver (Street Trees, 2024). For this analysis, we will use AWS Cloud Platform considering data analytics tools such as Glue, Data Brew, and S3 to process the data. First, we will load the raw data into S3 (ingestion). Then, we will clean and profile the data using Data Brew to remove any missing values, duplicates, or unnecessary columns, ensuring the data is ready for analysis. Finally, we will design an ETL pipeline using AWS Glue to transform and extract actionable insights. The following image illustrates the operational workflow: 

![street-trees-drawio](https://github.com/user-attachments/assets/cb4705d8-e72f-4311-ba7f-99a2da9284cc)

# Descriptive Analytics
1. *Project Description*: Identifying the most frequent street for tree planting to plan maintenance and future planting strategies.
2. ###Project Title: Highlighting popular street having trees.
3. ###Objective: This data can help the city prioritize streets with greater capacity for trees get sufficient attention for maintenance such as watering, pruning, pest control while promoting environmental equity

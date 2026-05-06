# Modernizing Data Lakehouse

## Objective
The objective of this project is to modernize data lakehouse infrastructure using tools such as Dremio, MinIO, and Alteryx, while improving and accelerating the eligibility process through machine learning methods.

## Data Engineering

In this project, Dremio were used as the query engine, MinIO as Object Storage, and Alteryx as verfication processs and machine learning. 

### Legacy Architecture

![image](images/Legacy_Architecture.png)

- Microsoft SQL Server (MSSQL) serves as the primary data source for this project, while Microsoft Excel is currently used as an ETL tool despite its scalability limitations. The processed data is then stored in a data warehouse, where it undergoes validation by the Data Verification Team before being analyzed and presented to managers to support data-driven decision-making.


### Modern Architecture

![image](images/Proposed_Architecture.png)

- Data is ingested from multiple sources and transformed through an ETL pipeline before being stored in a scalable object storage system. Dremio then acts as the query engine, enabling efficient data access, analysis, and querying across the stored datasets.

![image](https://github.com/radzmi/STQD6324_Data_Management_Assigment1/assets/152348714/f6d841a6-7b7b-4d07-b901-2dd849436a1b)

- Some of the querying process in Dremio

## Machine Learning

![image](images/EDA.jpg)

- This is the EDA processs that already been done in Alteryx. The dataset is first loaded and filtered by selecting only the required columns. Rows containing null values are removed to ensure data quality, followed by renaming columns and adjusting data types for consistency. The data is then grouped based on relevant criteria before being exported in CSV format for further analysis or storage.


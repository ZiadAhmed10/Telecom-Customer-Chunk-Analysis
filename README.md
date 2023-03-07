# Telecom Customer Chunk Analysis

## PROJECT CONTEXT :

This sample data tracks a fictional telco company's customer churn based on a variety of possible factors. The churn column indicates whether or not the customer left within the last month. Other columns include gender, dependents, monthly charges, and many with information about the types of services each customer has. Source: IBM.

-------------------------------------------------
## Project data-set link : 
### https://docs.google.com/spreadsheets/d/1aGH3n-c6gSRFY5Mu7KNl7xXJDCM8KTIX/edit?usp=sharing&ouid=117338861444871771319&rtpof=true&sd=true
-------------------------------------------------
## Project objectives:
- EDA [Exploratory Data Anlysis]
- [Data Validation](#Data-Validation)
- Data Cleaning
- Data Manipulation and communicating my insights
- Designing a Dashboard
- Categorical Data Encoding
- Finding variables that impact churn Score

### Note :
Every screenshot you're going to see in this file is just a sample, And i implement the methodelagy that the screenshot contains on the whole dataset.


## Getting Started :
--------------------
1- Giving the columns more descriptive names to make it easier for me to understnad the data [With the help of Kaggle]

![image](https://user-images.githubusercontent.com/121814714/223100643-41d19618-9f2d-43e2-b836-16c8ea1bf9c4.png)
-------------------------------------------------
2- Formatting each table in a single tab in my file as a table 

![image](https://user-images.githubusercontent.com/121814714/223104260-9d314c1a-5e06-486e-8eaf-9cb689989848.png)
-------------------------------------------------
3- Renaming each of my tables in order to be having more descriptive names

![image](https://user-images.githubusercontent.com/121814714/223104641-b0a41c90-08f2-4a24-b668-23bf4deb08e9.png)
-------------------------------------------------
4- Checking for duplicates data 

![image](https://user-images.githubusercontent.com/121814714/223226127-291baf7a-6271-4b66-873f-ff469a3ed5ef.png)
-------------------------------------------------
5- Checking for missing data 

![image](https://user-images.githubusercontent.com/121814714/223420991-1dab007c-347d-4f92-ae8a-93d458d8a686.png)
-------------------------------------------------
6- Handelling missing data

- EX : Replacing missing data with logical values [Like in the screenshot below, It makes scence that 'Churn Label' for customers whose status is churned will be yes, And for customers whose status is stayed, It'll defintely be no]
![image](https://user-images.githubusercontent.com/121814714/223423817-ad947f28-b4f5-491d-bff0-079b67e86dfa.png)
-------------------------------------------------
- EX2: Replacing null values in 'Churn Category' with 'Not churned', As in this column the missing values indicate that this customer is not churned so there is no category for his churn
![image](https://user-images.githubusercontent.com/121814714/223426248-a5d4c746-b4f2-44d6-a805-09a29bc17b7e.png)
------------------------------------------------------------------------------------------------------------
### By now the data is validated and cleaned, missing values are handeled, there are no outliers, there are no duplicates.

### So, This is the time to ask questions in order to answer them to gain some insights about the data
## Questions that you'll find their answers through the project:
- [How many of my customers are chunked or stayed or joined?](#how-many-of-my-customers-are-chunked-or-stayed-or-joined)
- Why are people leave the company? [Chunk category]
- [Title headline](#title-headline)
- f
- f
------------------------------------------------------------------------
### How many of my customers are chunked or stayed or joined?

## Title headline




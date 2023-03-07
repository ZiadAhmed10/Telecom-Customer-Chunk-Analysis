# Telecom Customer Chunk Analysis

## `PROJECT CONTEXT` :

This sample data tracks a fictional telco company's customer churn based on a variety of possible factors. The churn column indicates whether or not the customer left within the last month. Other columns include gender, dependents, monthly charges, and many with information about the types of services each customer has. Source: IBM.

-------------------------------------------------
## `Project data-set link:` 
### https://docs.google.com/spreadsheets/d/1aGH3n-c6gSRFY5Mu7KNl7xXJDCM8KTIX/edit?usp=sharing&ouid=117338861444871771319&rtpof=true&sd=true
-------------------------------------------------
## `Project objectives:`
- EDA [Exploratory Data Anlysis]
- Data Validation
- Data Cleaning
- Data Manipulation and communicating my insights
- Designing a Dashboard
- Categorical Data Encoding
- Finding variables that impact churn Score

### Note :
Every screenshot you're going to see in this file is just a sample, And i implement the methodelagy that the screenshot contains on the whole dataset.


## `Getting Started :`
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
## `Questions that you'll find their answers through the project:`
- [How many of my customers are chunked or stayed or joined?](#how-many-of-my-customers-are-chunked-or-stayed-or-joined)
- [Why do people leave the company?](#why-do-people-leave-the-company)
- [What is the alarming churn scores group for my customers?](#what-is-the-alarming-churn-scores-group-for-my-customers)
- [Which quarter has the highest number of churned customers?](#which-quarter-has-the-highest-number-of-churned-customers)
- [Is there a relationship between customers gender and their status?](#is-there-a-relationship-between-customers-gender-and-their-status)
- [What is the number of each customer status per mirital status?](#what-is-the-number-of-each-customer-status-per-mirital-status)
- [Does the offers subscription have got something to do with customers status?](#does-the-offers-subscription-have-got-something-to-do-with-customers-status)
- [Does the inernet sevice that the company provide contribute into making customers leave the company?](#does-the-inernet-sevice-that-the-company-provide-contribute-into-making-customers-leave-the-company)
------------------------------------------------------------------------
### How many of my customers are chunked or stayed or joined?
![image](https://user-images.githubusercontent.com/121814714/223470705-39e96476-dc95-436e-9682-f3a3e030ff6f.png)
------------------------------------------------------------------------
### Why do people leave the company?
![image](https://user-images.githubusercontent.com/121814714/223470791-ab063fbd-5626-496d-9a17-059b8a7c04c6.png)
------------------------------------------------------------------------
### What is the alarming churn scores group for my customers?
- Creating a column in my dataset that depend on 'Churn score' column's values utilizing IF condition, In order to create 10 bins of churn scores to make it easier to explore and analyze the data.
- It's obvious that 'Churned' status in my customers started showing up in (56 : 65) churn score group which makes this scores group the turning point for my customers.
![image](https://user-images.githubusercontent.com/121814714/223489191-6fc5b4fd-4cb8-4a72-8026-82a9f5c9b0f4.png)
------------------------------------------------------------------------
### Which quarter has the highest number of churned customers?
- Almost all churned customers, They became churned in Q3 and that's because of the dataset, As the dataset has only 3 observational rows in Q1 and Q2

![image](https://user-images.githubusercontent.com/121814714/223496683-0a125b26-05ba-4de6-8f69-f91983b2c4d7.png)
------------------------------------------------------------------------
### Is there a relationship between customers gender and their status?
- So, Obvisouly Customers' gender has nothing to do with their status
![image](https://user-images.githubusercontent.com/121814714/223502303-519c8c7a-a35b-425c-a2fe-2edb8fe93645.png)
------------------------------------------------------------------------
### What is the number of each customer status per mirital status?
- It's obvious that churned people who are not married are almost double the number of churned people who are married
![image](https://user-images.githubusercontent.com/121814714/223516944-8d943e44-34d9-42d6-911a-b7d7d066f90b.png)
------------------------------------------------------------------------
### Does the offers subscription have got something to do with customers status?
- It's very clear that people who don't subscribe to offers are the most to leave the company! So the company may target them through customzing special offers to them, So their loyality increases by the time

![image](https://user-images.githubusercontent.com/121814714/223525078-9dd38133-d79b-4165-ad17-61ee8900d527.png)
-----------------------------------------------------------------------------
###  Does the inernet sevice that the company provide contribute into making customers leave the company?
- Numericals say that most of our churned customers were subscribed to our internet service [15 double the number of churned people who didn't discribe to the company internet service], Which indicates that the company has an URGENT ALARM regarding its internet service
- `Note` : Same URGENT ALARMING regarding phone service which is provided by the company, As there are 1699 out of 1869 churned ones who did subscribe to the home phone service.

![image](https://user-images.githubusercontent.com/121814714/223530771-d3368d8e-a6f6-40d0-9ee6-2895cb76f75e.png)
-----------------------------------------------------------------------------






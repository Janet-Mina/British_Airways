### British_Airways

---
### Table of Contents
1.  [Overview](#overview)
2. [Introduction](#introduction)
3. [Objectives](#objectives)
4. [Data source](#data-source)
5. [Skills Demonstrated](#skills-demonstrated)
6. [Modelling](#modelling)
7. [Visualizations](#visualizations)
8. [Insights](#insights)
9. [Recommendations](#recommendations)

---
### Overview
This repository contains a Power BI analysis of British Airways flight performance for a duration of six months. The analysis covers key performance indicators (KPIs), flight operations, and financial performance to provide actionable insights.

---
### Introduction
The British Airways is located in the United Kingdom, London and is the second largest UK based airline on fleet size(i.e. total number of aircrafts in an airline and total passengers carried). British Airways operates a vast network of flights and connects passengers to their destinations worldwide. 

---
### Objectives
The objective of this data is to answer the following questions:
1. Which manufacturer has the best aircrafts in terms of fuel_efficiency?
2. Does British Airways tend to use aircraft from manufacturers known for there superior fuel efficiency more frequently?
3. Which month did passengers cancel flights the most?
4. Which city do passengers travel to the most?
5. What is the revenue generated from baggage overtime?
6. What is the average number of passengers like for each month?
   
---
### Data source
The data used for this project are 4 different excel csv files [British_Airway](https://kaggle.com) viz; the flights table with different colums, the flight routes table, the fuel_efficiency table and aircraft table.

---
### Skills demonstrated
- Uing Microsoft Excel: Cleaned the data in all 4 tables by handling missing values, removing duplicates and standardized formats
- Using SQL: Created a database and also tables in other to import the tables from Excel into the SQL database.
  -  Queried the database to extract the results from the different questions asked by the organisation.
- Using Power BI:
  - Connected the SQL to Power BI server.
  - loaded the already cleaned tables to power query editor
  - Created a calendar table as well as different DAX formulas
  - reconnected the relationships in the data model
  - Designed different visuals for my dashboard as regards the questions being asked
  - Added tooltips to visuals
  
--- 
### Modelling
The model is a star schema, with one fact table and 3 dimensional tables. The dimension tables are joined to the fact table with a one-to-many relationship.
![](img/model.png)

---
### visualizations
This is a one page report dashboard. Alongside visuals of the SQL queries

**Dashboard**

The dashboard has 4 KPIs with growth percentages, 5 visuals of a line,bar,pie,map charts and 2 slicers.

![](img/BA_dashboard.png)

**Tables created in sql**
![](img/Tables.png)

1. Which manufacturer has the best aircrafts in terms of fuel_efficiency?

| Query                        |                      Results |
|----------------------------- | -----------------------------|
|![](img/Q1.png)               |        ![](img/Q1_answer.png)|


2. Does British Airways tend to use aircraft from manufacturers known for there superior fuel efficiency more frequently?

| Query                        |                      Results |
|----------------------------- | -----------------------------|
|![](img/Q2.png)               |        ![](img/Q2_answer.png)|

3. Which month did passengers cancel flights the most?
   
| Query                        |                      Results |
|----------------------------- | -----------------------------|
|![](img/Q3.png)               |        ![](img/Q3_answer.png)|

4. Which city do passengers travel to the most?
   
| Query                        |                      Results |
|----------------------------- | -----------------------------|
|![](img/Q4.png)               |        ![](img/Q4_answer.png)|

5. What is the revenue generated from baggage overtime?
   
| Query                        |                      Results |
|----------------------------- | -----------------------------|
|![](img/Q5.png)               |        ![](img/Q5_answer.png)|

6. What is the average number of passengers like for each month?
    
| Query                        |                      Results |
|----------------------------- | -----------------------------|
|![](img/Q6.png)               |        ![](img/Q6_answer.png)|

---
### Insights
The British Airways flight data for January to June,2023 has incomplete data for the month of June.

Total flight: **1,012**

Total passengers: **105,000**

Total baggage revenue: **34,084,625**

Average passenger: **104**

- From the data gotten, British Airways has 14 aircrafts from 5 maunfacturers(Boeing, Airbus, Mitsubishi,Embraer and Sukhoi) having varying fuel_efficiency value.
Airbus has a manufacturer has 3 aircrafts,Embraer has 2 aircrafts,sukhoi has 1 aircraft, Boeing has 7 aircrafts and Mitsubushi has 1 aircraft. As a result of some manufacturers having more than one aircraft the average fuel-efficiency of all 14 aircrafts was calculated and Mitsubishi had the lowest average fuel-efficiency

  | Manufacturer  | Avg fuel-efficiency |
  | --------------|-------------------- |
  | Mitsubishi    |	0.021              |
  | Boeing	      |  0.029              |
  | Sukhoi	      |  0.043              |
  | Embraer	      |  0.053              |
  | Airbus	      |  0.579              |

- British airways tend to use aircraft  from manufacturers known for their superior fuel-efficiency more often. From the 5 manufacturers only 3 manufacturers(Airbus, Boeing and Embraer) were used. Boeing manufacturer has 2 aircraft subtype with low fue

---
### Recommendations
- A lower fuel_efficiency value indicates better performance because it shows less fuel is needed to travel a long distance. Therefore, Mitsubishi having the less value fuel_efficiency value of *0.021* is considered to be the best fuel_efficient aircraft and should be used.


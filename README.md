# Google-Query

## Project Overview
I’ve been exploring how to use QUERY to make working with data more efficient and easier. This repository documents what I’ve learned so far.

Google Sheets QUERY is like SQL inside a spreadsheet. It allows you to filter, sort, and analyze data with powerful functions. 

## Data Sources
The data was gotten from an open data source called Google Sheets. [Download Here](https://docs.google.com/spreadsheets/d/11VOyqzG1FfVxIKcNZ9iAH2_Nv5OHhFxzlhI2Ag4e8_A/edit?usp=sharing)

## Tools Used
- Google Sheets for Querying of Data
- Github for Portfolio Building
  

## What I Have Learnt:
 Here’s a breakdown of key functions I’ve been practicing:
- Using SELECT to choose retrieve columns of data.
```
SQL STATEMENT

 =QUERY(A1:H44,"SELECT *",1)
```
Sorting data in either Ascending or Descending with ORDER BY to make it easier to analyze.
```
SQL STATEMENT

=QUERY(A1:H44,"SELECT B,H,F WHERE B='Richard' AND F=2014 ORDER BY H DESC",1)
``` 
Restricting results with LIMIT to focus on just the most important data
```
 SQL STATEMENT

=QUERY(A1:H44,"SELECT A,B,H,F WHERE F=2014 ORDER BY H DESC LIMIT 10",1)
```
Finding specific information with LIKE to match patterns in data.
```
SQL STATEMENT

=QUERY(A1:H44,"SELECT A,B WHERE B LIKE 'R%'",1)
```
Combining conditions with AND and OR to get exactly the data I need
```
SQL STATEMENT

=QUERY(A1:H44,"SELECT C,D,E,F WHERE D LIKE '%_4'AND (E='Jul' OR E='Dec') AND F=2014",1)
```
Filtering data with WHERE to show only the rows that meet certain conditions.
```
SQL STATEMENT

=QUERY(A1:H44,"SELECT A,C,H WHERE H<100",1)
```
Summarizing data with AGGREGATE functions like SUM, AVG, MIN AND MAX
```
SQL STATEMENT

=QUERY(A1:H44,"SELECT SUM(H),MAX(H),MIN(H),AVG(H)",1)
```
<img width="654" alt="query 1" src="https://github.com/user-attachments/assets/7f0fdf4f-7e7e-4d82-bb9d-35ccefb391e1">

One of the main benefits I’ve experienced is easier data management. I can retrieve and manipulate data more efficiently, saving me time to explore the data by organizing and filtering large datasets. I can identify trends and patterns and gain better insights.

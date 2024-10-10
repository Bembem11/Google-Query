# Google-Query

## Project Overview
I’ve been learning more about Google Sheets QUERY, which is a great tool for analyzing, transforming data similar to SQL but in Google Sheets

## Data Sources
The data was gotten from an open data source called Google Sheets. [Download Here](https://docs.google.com/spreadsheets)

## Tools used
- Google Sheets for Querying of Data
- Github for Portfolio Building

I have been learning about making queries on Google sheets:
- Using SELECT to choose retrieve columns of data.
```
SQL STATEMENT =QUERY(A1:H44,"SELECT *",1)
```
Sorting data in either Ascending or Descending with ORDER BY to make it easier to analyze.
```
SQL STATEMENT =QUERY(A1:H44,"SELECT B,H,F WHERE B='Richard' AND F=2014 ORDER BY H DESC",1)
``` 
Restricting results with LIMIT to focus on just the most important data
```
 SQL STATEMENT =QUERY(A1:H44,"SELECT A,B,H,F WHERE F=2014 ORDER BY H DESC LIMIT 10",1)
```
Finding specific information with LIKE to match patterns in data.
```
SQL STATEMENT =QUERY(A1:H44,"SELECT A,B WHERE B LIKE 'R%'",1)
```
Combining conditions with AND and OR to get exactly the data I need
```
SQL STATEMENT =QUERY(A1:H44,"SELECT C,D,E,F WHERE D LIKE '%_4'AND (E='Jul' OR E='Dec') AND F=2014",1)
```
Filtering data with WHERE to show only the rows that meet certain conditions.
```
SQL STATEMENT =QUERY(A1:H44,"SELECT A,C,H WHERE H<100",1)
```
Summarizing data with AGGREGATE functions like SUM, AVG, MIN AND MAX
```
SQL STATEMENT =QUERY(A1:H44,"SELECT SUM(H),MAX(H),MIN(H),AVG(H)",1)
```


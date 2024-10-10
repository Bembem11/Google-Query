# Google-Query

## Project Overview

## Data Sources
The data was gotten from an open data source called Google Sheets

## Tools used
- Google Sheets
- Github for Portfolio Building

I have been learning about making queries on Google sheets
- Using SELECT to choose retrieve columns of data.
```
SQL STATEMENT 
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
              =QUERY(A1:H44,"SELECT B,C WHERE B LIKE '%an%'",1)
```

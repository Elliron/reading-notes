# Database Normalization
  - process used to organize a database into tables and columns
  - table should be about specific topic
  - spreadsheet
  - limiting a table reduces number of duplicate data
  - eliminates some issues of modification
  - reasons for normalization
    - minimize duplicate data
    - minimize or avoid modification issues
    - simplify queries

## 3 normal forms
  - 1nf, 2nf, 3nf
  - less prone to modification issues
  - First Normal Form
    - info stored in table with each column containing atomic values, no repeating groups of columns
  - Second Normal Form
    - In first form and all columns depend on primary key
  - Third Normal Form
    - in second form and all columns not transitively dependent on primary key

## Data Duplication and Modification
  - increases storage
  - decrease performance
  - difficult to maintain changes


[Home](../README.md)
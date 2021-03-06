# Database Normalization

> Database normalization is a process used to organize a database into tables and columns

- table should be about a specific topic
- There are three normal forms most databases adhere to using.
- As tables satisfy each successive database normalization form, they become less prone to database modification anomalies

### 3 main reasons for database normalization

1. minimize duplicate data
2. minimize or avoid data modification issues
3. simplify queries

You want tables to have **one** purpose.

### 3 database modification anomalies 

1. Insert Anomaly
2. Update Anomaly
3. Deletion Anomaly

### 3 common forms of database normalization

- There are three common forms of database normalization: 1st, 2nd, and 3rd normal form. They are also abbreviated as 1NF, 2NF, and 3NF respectively

- The forms are progressive, meaning that to qualify for 3rd normal form a table must first satisfy the rules for 2nd normal form, and 2nd normal form must adhere to those for 1st normal form

- **First Normal Form** – The information is stored in a relational table with each column containing atomic values. There are no repeating groups of columns.
- **Second Normal Form** – The table is in first normal form and all the columns depend on the table’s primary key.
- **Third Normal Form** – the table is in second normal form and all of its columns are not transitively dependent on the primary key



# Stuff I Learn: Tracking My Learning Journey

Welcome to my learning journey! Here, I document the snippets of knowledge I acquire along the way.

---

## SQL

### Selecting a Database
```sql
USE some_database;
```

### Selecting a Complete Table
```sql
SELECT * FROM some_table;
```
### Selecting Specific Columns

```sql
SELECT column1, column2 FROM some_table;
```

### Selecting Unique Values in a Column

```sql
SELECT DISTINCT column1 FROM some_table
```
### Creating a New Calculated Column

```sql
SELECT existing_column, existing_column + 10 AS 'Existing Column Plus Ten' FROM some_table;
```

### Conditional Selection (Selecting all rows where the column1 value is equal to 'sepehr')

```sql
SELECT column1, column2 FROM some_table WHERE column1 = 'sepehr';
```
### Ordering The Table

```sql
SELECT * FROM some_table ORDER BY some_column;
```

### Commenting Out a Line

```sql
-- SELECT * FROM some_table;
```
### Selecting Rows by a Specific Year (Assuming the date format is YYYY-MM-DD)

```sql
SELECT * FROM some_table WHERE YEAR(date_column) = 2019;
```

### Using IN for Multiple Value Matches (Selecting only rows where some_column is equal to 'value1' or 'value2')
```sql
SELECT * FROM some_table WHERE some_column IN ('value1', 'value2');
```

### Using AND and OR in Filtering (Selecting rows where either the first_name is 'Babara' or the last_name is 'Betchley')

```sql
SELECT * FROM customers WHERE first_name = 'Babara' OR last_name = 'Betchley';
```

### Selecting Rows With Value In a Range

```sql
SELECT * FROM some_table WHERE quantity BETWEEN 100 AND 1000;
```

### Selecting Only Rows Starting With 'a'
```sql
SELECT * FROM some_table FROM some_column LIKE 'a%'
```

### Selecting Only Rows Starting With 'a' And ending With 'y'
```sql
SELECT * FROM some_table FROM some_column LIKE 'a%' AND some_column LIKE '%y'
```

### Selecting Only Rows With Five Characters And Starting With 'a'
```sql
SELECT * FROM some_table FROM some_column LIKE 'a____'
```

### Selecting Only Rows Containing Character 'a':
```sql
SELECT * FROM some_table FROM some_column LIKE '%a%'
```

### Matching Wth Regular Expression
```sql
SELECT * FROM some_table FROM some_column REGEXP 'some_text'
```

### Selecting Rows That Their some_column Value Starts With 'm' Or Ends With 'y'

```sql
Select * FROM some_table WHERE some_column REGEXP '^m|y$'
```

### Selecting Rows That Their some_column Value contain 'ey' Or 'ay'

```sql
SELECT * FROM some_table WHERE some_column REGEXP '[ea]y'
```
### Selecting Null Rows
```sql
SELECT * FROM some_table Where some_column IS NULL
```
### Ordering a Table Based On Specific Column In Descending Order
```sql
SELECT * FROM some_table ORDER BY some_column DESC
```

### Limiting Number Of Rows
```sql
SELECT * FROM some_table LIMIT 3
```

### Selecting Specific Rows (skip 6 then select three)
```sql
SELECT * FROM some_table LIMIT 6,3
```

### Joining Columns of a Table to Some Other Table
```sql
SELECT s1.column1,s1.column2 FROM some_table1 s1 JOIN some_table2 s2 ON s1.column1=s2.column1
```


### Joining Columns of a Table to Some Other Table Based On a Join Condition With Exactly The Same Column Name
```sql
SELECT s1.column1,s1.column2 FROM some_table1 s1 JOIN some_table2 s2 USING(column_name)
```

### Cross Joining Columns of a Table to Some Other column
```sql
SELECT t1.some_column,t2.some_column from table1 t1 cross join table2 t2 order by t1.some_column
```
### Doing a Union on Two Tables
```sql
SELECT * from table1 UNION SELECT * from table2
```
### Inserting a Single Row to a Table
```sql
INSERT INTO some_table VALUES(DEAFULT,'some_value')
```
### Inserting a Single Row to a Table, Only Filling Specific Columns
```sql
INSERT INTO some_table (column1,column3) VALUES(value1,value2)
```
### Creating a Copy of a Table 
```sql
CREATE TABLE new_table_name AS SELECT * FROM some_old_table_name
```
### Updating a Table 
```sql
UPDATE some_table SET column1=blah_blah,column2=blah where column3=blah_blah_blah```
```
### Deleting 
```sql
DELETE FROM some_table where some_column='something'
```
---
## REGEX

### Match Chatacters Ending With Something
```REGEX
'some_word$'
```

### Match Chatacters Starting With Something
```REGEX
'^some_word'
```

### Match words Containing Character 'r' With a,b,c,d After That
```REGEX
'r[a-d]'
```
### Matching Words Containing char1 Or char2

```REGEX
'char1|char2'
```

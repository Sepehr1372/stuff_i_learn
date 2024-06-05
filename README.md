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

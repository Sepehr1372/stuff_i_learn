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

###Using AND and OR in Filtering (Selecting rows where either the first_name is 'Babara' or the last_name is 'Betchley')

```sql
SELECT * FROM customers WHERE first_name = 'Babara' OR last_name = 'Betchley';
```


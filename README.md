# stuff_i_learn: things i learn every now and then

#SQL>>
# selecting a database
USE some_database

# selecting a complete table from a database
SELECT * FROM some_table

# selecting specific columns from a table
SELECT column1,column2 FROM some_table

# making a column unique (no duplicates)
SELECT DISTINCT column1 FROM some_table

# creating a new column from some alreaady existing column
SELECT existing_column,existing_column+10 AS 'existing column plus ten' FROM some_table

# conditional selecting (select all rows that its coloumn1 value is equal to 'sepehr')
SELECT column1,column2 FROM some_table WHERE column1='sepehr'

# ordering the table 
SELECT * FROM some_table ORDER BY some_column

# commenting out a line
-- SELECT * FROM some_table

# selecting rows with a specific year (the year format is like this 2019-04-04)
SELECT * FROM some_table WHERE YEAR(date_column)='2019'

# IN (selecting only rows which its column value is equal to value11 OR value2)

# using AND and OR in filtering 
SELECT * FROM customers WHERE first_name='Babara' OR last_name='Betchley'

# selecting only rows thats its some_column value is equal to 'value1' OR 'value2'
SELECT * FROM some_table WHERE some_coloumn in ('value1','value2')

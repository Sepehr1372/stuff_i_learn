# stuff_i_learn: things i learn every now and then

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

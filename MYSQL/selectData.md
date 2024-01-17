# To select data from table

select statement 
    - `SELECT`, It is used to select the columns
    -  `TOP`, select the top few rows in table (eg. SELECT TOP 400 FROM *)
    -  `DISTINCT`, SELECT unique element
    -  `COUNT`, count total number of element present 
    -  `AS`, TO give name alias to new column
    -  `MAX`, TO check the maximum value 
    -  `MIN`, To check minimum value
    -  `AVG`  To check the average value

1. to select whole table
   1. `SELECT * FROM tableName`
2. To select perticular column from table
   1. `SELECT columnName FROM tableNAme`
3. To select top few rows
   1. `SELECT TOP numberOfTopRows ColumnName FROM tableName`
4. TO select unique element from table
   1. `SELECT DISTINCT(columnName) FROM TableNAme`
5. To count total number of element poresent in Column
   1. `SELECT COUNT(columnNAme) FROM TabelNAme`
6. TO give alias to column
   1. `SELECT COUNT(columnNAme) AS AliasName FROM TableNAme`
7. TO check maximum value 
   1. `SELECT MAX(ColumnName) From TableName `

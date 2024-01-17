
# Create empty Table with columns

`CREATE TABLE tableName (
    columnName1 type,
    columnName2 type
)`

### example

`CREATE TABLE employeeDemographics
(EmployeeId int,
FirstName charVar(50),
LastName charVar(50),
Age int)`



# Adding data to this empty table

`INSERT INTO tableName(column1_value column2_value column3_vale)`

### example

- To insert single row of data
`INSERT INTO employeeDemographics
(1001, 'AJ', 'KR', 23)`

- TO insert multiple rows
  - `INSERT INTO employeeDemographics
((1001, 'AJ', 'KR', 23),
(1002, 'BJ', 'KJ', 34))`


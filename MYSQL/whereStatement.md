
# use Where Statement

Where Statement
    1. `WHERE` Limits amount of data, and specify the data you want to return
    2. `<>`  not equal
    3. `=` Equal
    4. `<` smaller then
    5. `>` greadter then
    6. `"` 
    7. `AND` join multiple operation with and operation
    8. `OR`  join multiple operation with or operation
    9. `LIKE`   check docs , used sometimes for numeric but mostely string.
    10. `NULL`
    11. `NOT NULL`
    12. `IN` its like multiple equal statement
   

1. TO select column who satisfy codition 
   1. `SELECT columnName From TableNAme WHERE condition`
2. to select column lets say NAME, whoise name starts with s
   1. `SELECT * From TableName WHERE Name LIKE 's%`  here % is wildcard
3. TO select multiple value from a column
   1. `SELECT * From TableNAme WHERE NAME in ('JIM','AJ','SAM')`
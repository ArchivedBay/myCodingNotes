# This file will showcase common SQL commands and concepts learned.

## Basic Commands ##
  - ```CREATE DATABASE <databaseName>``` - Creates a new Database with the specified name
  - ```USE <databaseName>``` - Set the specified Database as the currently active Database to query.
  - ```SHOW DATABASES``` or ```SHOW TABLES``` - Shows a list of available databases, or tables linked to the current DB.
  - ```SELECT``` - Grabs information from the specified table. More on this later.
  - ```UPDATE``` - Updates information on the specified table. More on this later.
  - ```DROP TABLE <tableName``` or ```DROP DATABASE <databaseName>``` - Delete the specified table or Database. 
  
## using SELECT ##
  - When using SELECT you can specify certain information to search against.
  - take the following example:
    - ```SELECT firstName, lastName FROM listOfPeople;```
      - in the above, firstName and lastName are "fields" that were specified when the ```listOfPeople```table was created.
    - ```SELECT * FROM listOfPeople;```
      - this would return the entire table itself, and all the data in it.
    - ```SELECT firstName FROM listOfPeople WHERE id = 1;```
      - this would return ONLY the ```firstName``` field of the row in ```listOfPeople``` where ```id``` was = to 1.
    - You can also have an indented version, in say an SQL file. this is what I tend to prefer doing:
      - ```   
        SELECT
            id,
            CONCAT(firstName, ' ', lastName) AS 'Name',
            favouriteFood
        FROM <tableName> WHERE id < 4;```
      - this will return a table that would concat the values of the ```firstName``` and ```lastName``` 
        fields in the <tableName> table, AS a single field called 'Name', and then also display the 
        ```id``` and ```favouriteFood``` fields, for EVERY row where the id is less than 4, so 1(or 0 if you have something at 0)-3.
        The following is the output given when you run this query:
        
        ![Code shown](https://i.imgur.com/Y82StrE.png)
              
              

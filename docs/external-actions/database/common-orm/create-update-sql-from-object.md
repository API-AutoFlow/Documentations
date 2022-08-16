---
layout: default
title: Create Update SQL from Object
parent: Common ORM
grand_parent: Database
---

# Create Update SQL from Object
{: .no_toc }

Sequelize object action to convert Object into an Update SQL.

## Properties
Object: The object with both the column (object key) and the values to be updated
Table: Name of the table to insert the data
id-name: WHERE clause condition (column)
id-value: WHERE clause condition  (value)

## Output
Output-location: Response from the database

### Example
Given below object
```
{ “column1”: “value1”,  “column2”: “value2”,  “column3”: “value3”}
```

table: table_name

id_name : id_name

id_value : id_value

The SQL query will be generated
```
UPDATE table_name
SET column1 = value1, column2 = value2, column3 = value,
WHERE id_name = id_value;
```

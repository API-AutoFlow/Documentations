---
layout: default
title: Create Insert SQL from Object
parent: Common ORM
grand_parent: Database
---

# Create Insert SQL from Object
{: .no_toc }

Sequelize object action to convert Object into an Insert SQL.

## Properties
Object: The object with both the column (object key) and the values to be inserted
Table: Name of the table to insert the data

## Output
Output-location: Response from the database

### Example
Given below object

```
{ “column1”: “value1”,  “column2”: “value2”,  “column3”: “value3”}
```

Table : table_name

The SQL query will be generated

```
INSERT INTO table_name (column1, column2, column3)
VALUES (value1, value2, value3);
```

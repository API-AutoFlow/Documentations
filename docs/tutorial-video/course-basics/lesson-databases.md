---
layout: default
nav_order: 6
title: Lesson 6 Database
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 6 min video
<h1 style="margin-top:0">Lesson 6: Learn How to Work with Databases</h1>

Now with a good understanding of `iteration`, you can start working with the database.
A database returns a list of records in an array format.

<iframe width="560" height="315" src="https://www.youtube.com/embed/u4B_KeqIrY4" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

**Prerequisite**: 

* [Learn how to make SQL query](https://www.w3schools.com/sql/sql_syntax.asp)
* [MySQL Installation](/docs/tutorial-video/course-supplementary/mysql/)


## Lesson Outline

1. Apply `database` action to the `flow`
2. Fill out the `database` action settings
3. Apply the `iteration` actions

## 1\. Apply `database` action to the `flow`

![Apply database action](/assets/images/database-tutorial.png)

Learn more about [database](/external-actions/database/mariadb) action

## 2\. Fill out the `database` action settings

Use `single execution` for the current use case. But you can also [use database connection](#use-database-connection) if you are planning on calling the database multiple times.

![Fill out database action](/assets/images/database-tutorial-1.png)

## 3\. Apply the `iteration/foreach` actions

The database returns the data in an array.  Use `iteration` action to loop over the array.

For this use case, we will use [iteration/for-each](/internal-actions/iteration/foreach) action to apply actions for each of the items in the array.

![Apply iteration for each](/assets/images/database-tutorial-2.png)

Learn more about [iteration/for-each](/internal-actions/iteration/foreach) action

## 4\. Create an empty `array` by applying a `data/set` action

In most use cases, the data from the database needs to be transformed into another format.

Use `data/set` action to create an empty array to store the newly looped data.

![Create an empty array](/assets/images/database-tutorial-3.png)

## 5\. Put together a new dataset by applying an `array/insert-at` action

For each item, use [array/insert-at](/array/insert-at) action to insert the newly formed data in the empty array that was created in the previous step. 

Note that the action is creating a new object with a new object `key`.

To change the value, use the string actions since the data is in string format. 

![Use array insert at](/assets/images/database-tutorial-4.png)

Learn more about [array/insert-at](/array/insert-at) action

## 6\. Put together a response by applying a `data/set` action

Finally, to provide the data for others to use, final data needs to be provided in the `response/body`.

![Put together HTTP response](/assets/images/database-tutorial-5.png)


{% include in_line_banner_config.html config_title="Learn How to Work with Databases" config_url="/assets/configs/config-course1-lesson6-database.json" %}

***

## Create DATABASE

[How to install MySQL](https://www.simplilearn.com/tutorials/mysql-tutorial/mysql-workbench-installation)

MySQL example

```sql
CREATE DATABASE patients;
USE patients;
CREATE TABLE patient(
    id                BIGINT             AUTO_INCREMENT,
    name              VARCHAR(255)       NOT NULL,
    dob               VARCHAR(255)       NOT NULL
);

INSERT INTO patients.patient (name, dob) VALUES ("Peter Jung", "1990-01-01");
```

***

## Advanced

### Use Database Connection

When you are using the same database connection multiple times, you can create the connection once and apply to use the `use database connection` type.

## 1\. Create database connection

![Create database connection](/assets/images/database-tutorial-6.png)

## 2\. Fill in the database connection details

![Fill in the database connection details](/assets/images/database-tutorial-7.png)

## 3\. Check that the database connection is established

![Check database connection](/assets/images/database-tutorial-8.png)

## 4\. Select `use database connection` type

Select `database-id`

![Selece use database connection](/assets/images/database-tutorial-9.png)

{% include in_line_banner_config.html config_title="Learn How to Work with Database Connection" config_url="/assets/configs/config-course1-lesson6-databaseconnection.json" %}

[NEXT >> Lesson 7: Reusable Custom Actions, Files, and Data.  Cut and Paste Configurations](/docs/tutorial-video/course-1-basics/lesson-7-httprequest/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

{: .fs-6 .fw-300 }
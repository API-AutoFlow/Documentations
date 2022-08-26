---
layout: default
title: Lesson 1 API AutoFlow Basics
parent: Course 1 Getting Started
grand_parent: Tutorials - Video
---
<h6>Course 1: Getting started with API AutoFlow</h6>
<h1 style="margin-top:0">Lesson 1: API AutoFlow Basics</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/DBaNoZF2KIg" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Lesson Outline

* Go to Interactor website to access API AutoFlow
* Go through some of the definitions
* Overall how to navigtate and use the product
* And create a Hello World solution together 

## Get API AutoFlow
1. Go to www.interactor.com
2. Click the download button from the Product > API AutoFlow page

### Templates
Based on the product you are building, you can select from the pre-made templates.


## Using API AutoFlow Cloud
1. Click the Cloud button or go directly to console.apiautoflow.com
2. Register.  You will receive an confirmation email
Note: your ID becomes part of your URL endpoint
For example, for user with id John will be allocated a URL of api.apilautoflow.com/john

## Using API AutoFlow on-premise
Follow the installation instructions on the website

—-------

## Definitions
You can think of API AutoFlow as a factory that processes data.  If you think about it, that is what the backend is.

* Solution:  You can think it as a factory. The solution refers the entire backend
* Flow:  You can think of it as a process line for the data.  
* Actions: You can think of it as the workers who make changes to the raw materials
* Server: You can think of this as the freigh receiving dock
* Endpoint: You can think of this as the start of processing line
* Data: You can think of this as the raw material
* Simulation: You can think of it as the sample raw material
* Flow Transaction Data: You can think of it as the raw material that passes through the process line.  As changes are made by * the actions, the flow transaction data would change as it goes down the flow.

—-----------

## How to use API AutoFlow
API AutoFlow is divided into three panes.

* **Navigation (Left)**:  Tabs to each sections. Components are created the sections to be used in the solution.
* **Workspace (Center)**: Center is the workspace where most of the creation is done.
* **Components (right)**: You drag things from the right pane and apply it to the workspace

## How to make a solution
Let’s create a Hello World! solution 

1. Click on the Solution tab on the left navigation pane
2. Create a HTTP server by clicking on the drop down
3. Create an Endpoint by clicking on the same drop down and selecting the server just created
4. From the right pane, drag and drop the dataset action from the data category.
<br />
Note: dataset action simply sets a value to the solution flow.
5. In the settings for the action, enter Hello World! In the properties and in the output enter response > body





{: .fs-6 .fw-300 }
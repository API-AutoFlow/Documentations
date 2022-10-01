---
layout: default
nav_order: 3
title: Lesson 3 Data Simulation
parent: Course 1 Basics
grand_parent: Tutorials - Video
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 10 min video
<h1 style="margin-top:0">Lesson 3 Using Data Simulation for Easier Development</h1>

One of the most repetitive tasks as a solution maker is testing the features as you build them.

Wouldn't it be great if the solution automatically tests itself as you build the features?

That's what the data simulation feature of API AutoFlow does.

<iframe width="560" height="315" src="https://www.youtube.com/embed/EhuCs1kdCdM" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

Mock data is simulated or made-up data for the purpose of testing the solution during development.

Note: **Simulated data ONLY exists within the product**. This means, when testing outside API AutoFlow using your application or tools such as Postman will not have access to the simulated data.

## Lesson Outline

1. Flow Test Simulation (Flow Transaction Data)
2. Action Responce Simulation

## 1. Flow Test Simulation

The flow test simulation is a means of mocking the flow's input data.
For example, for HTTP, the input data would be the HTTP request and the output would be the HTTP response.

HTTP server attached flows, a user can simulate HTTP request and see what the HTTP response would be after the flow is complete.

IMPORTANT:  Dev Mode needs to be switched on to use the flow test simulation

![flow test simulation](/assets/images/flow-data-simulation.png)

### Setup the action to echo
Use the `data/set` action 
1. input *value* is the HTTP-request-body 
2. output is HTTP-response-body

![Flow copy HTTP request to response](/assets/images/flow-copy-http-request-to-response.png)

### Multiple simulation versions

When creating a solution, there are times when the user needs to test with multiple data sets.

By, pressing the `+` button, you can create as many versions of the test as you need.

![flow test simulation create](/assets/images/flow-data-simulation-create.png)

Use the drop-down to select the version of the flow test simulation.

![flow test simulation select](/assets/images/flow-data-simulation-select.png){: width="500px" }

Note: You can delete or pin a version with the buttons provided.


## Flow Transaction Data
The process of creating a flow is to design a chain of actions that provides desired response to the request.  

By simulating the request data within the product, developers can visualize the expected response as the flow is built and actions are applied.

The flow transaction data is on the **_bottom of the left navigation pane_**

**Key point**
1. Data received by the selected action
2. Stored in memory

![Flow transaction data](/assets/images/flow-transaction-data.png){: width="500px" }

## 2. Action Response Simulation

**Calling external data sources frequently can be a problem**

During solution making, it may not be ideal to execute those actions too many times for reasons such as rate limiting and slow responses delaying the development process.

Actions that interacts with an external source as a feature to simulate data.  This allows the solution maker to use `mocked` data during the `development mode`

![Action mock data](/assets/images/action-mock-data.png){: width="500px" }

Note: 
1. The mock data feature is checked by default.  Be sure to uncheck if you want to test with a real dataset
2. The mock data only exists within the API AutoFlow product. Mock data can not be used outside the product.

## How to Easily Create Mock Dataset

1\. Uncheck the mock data to get the real data
 
![Action mock data](/assets/images/action-mock-data-copy-paste-1.png){: width="500px" }

2\. Copy the data from the `flow transaction data`

![Action mock data](/assets/images/action-mock-data-copy-paste-2.png){: width="500px" }

3\. Check the mock data to simulate the data

![Action mock data](/assets/images/action-mock-data-copy-paste-3.png){: width="500px" }

4\. Paste the data into the mock data

![Action mock data](/assets/images/action-mock-data-copy-paste-4.png){: width="500px" }

{% include in_line_banner_config.html config_title="Using Data Simulation for Easier Development" config_url="/assets/configs/config-simulation.json" %}

[NEXT >> LESSON 4: Using Data Simulation for Easier Development](/docs/tutorial-video/course-1-basics/lesson-4-conditionals/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


{: .fs-6 .fw-300 }
---
layout: default
nav_order: 2
title: Lesson 2 Hello World!
parent: Course 1 Basics
grand_parent: Tutorials - Video
---
<h6>Course 1: Getting started with API AutoFlow</h6>
4 min read · 16 min video
<h1 style="margin-top:0">Lesson 2: Navigation and Hello World!</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/nZ_XeHXl2eY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Lesson Outline
1. Overall how to navigate and use the product
2. Create a Hello World solution together 

## How to use API AutoFlow
API AutoFlow is divided into five (5) panes.

![Navigation Panes](/assets/images/navigation-panes.png)

* [A] **Navigation (Left)**:  Tabs to each section. Components are created in the sections for use in the solution.
* [B] **Solution Canvas (Center-Top)**: Center-Top is the workspace where most of the creation is done.
* [C] **Settings (Center-Bottom)**: Setting pane for the selected actions, servers, and endpoints.
* [D] **Actions & Simulation (Right-Top)**: Collection of the actions that users can drag and drop to the Solution Canvas.  Data simulation is used to create mock data for each flow.
* [E] **Data, Log & Help (Right-Bottom)**: Snapshot of the selected action's data received. Logs for flows with action data/log are applied.  Help when the question icon is clicked.


## How to make a solution
Let’s create a Hello World! solution 

1\. Click on the Solution tab on the left navigation pane
2\. Create an HTTP server by clicking on the drop-down

![Create Server](/assets/images/create-solution-server.png){: width="600px" }

3\. Create an Endpoint by clicking on the same drop-down and selecting the server just created

![Create Ednpoint](/assets/images/create-solution-endpoint.png){: width="600px" }

4\. From the right pane, click on the **Actions** tab.

![Action tab](/assets/images/right-pane-action-tab.png){: width="600px" }

5\. click on the data category.

![Data category](/assets/images/actions-data-category.png){: width="600px" }

6\. Scroll down or search for **set** action and drag and drop to the solution canvas.

![Action Set](/assets/images/create-solution-action-set.png){: width="800px" }

<br />
Note: dataset action simply sets a value to the solution flow.

7\. Turn on the development mode to visualize the data

![Dev Mode](/assets/images/dev-mode-switch.png){: width="500px" }

8\. In the settings for the action, enter `Hello World!` in the properties and in the output enter response > body

![Actions Setting for Data Set](/assets/images/create-solution-data-set-settings.png){: width="800px" }

{% include in_line_banner_config.html config_title="Hello World!" config_url="/assets/configs/config-helloworld.json" %}

[NEXT >> LESSON 3: Data Simulation](/docs/tutorial-video/course-basics/lesson-data-simulation/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

{: .fs-6 .fw-300 }
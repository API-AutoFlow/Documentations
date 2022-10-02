---
layout: default
nav_order: 10
title: Lesson 10 Organization
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 9 min video
<h1 style="margin-top:0">Lesson 10: Organization</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/F80P-AIcGIs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Lesson Outline

1. Reusable Custom Actions
2. Copy Configuration
3. Paste Configuration
4. Import and Export Configuration
5. Roll Back
6. Organization

## 1\. Reusable Custom Actions

Create once and reuse many times. For developers, you can think of it as functions.  It takes an `input` and gives back an `output`.  You create a custom action using a flow just like you would in a solutions section. The custom action can be applied in any flow.

![Reusable Custom Actions](/assets/images/tutorial-custom-action.png){: width="500px" }

In the below example, a simple custom action with [data/set](/docs/internal-actions/data/set/) is configured.  The action takes in the `input` data and sets the response as the `output` data.

![Reusable Custom Actions](/assets/images/tutorial-custom-action-1.png){: width="800px" }

How the data flow is explained below. 

![Reusable Custom Actions](/assets/images/tutorial-custom-action-1-1.png){: width="600px" }

To apply the newly created custom action to the solution, go to actions **Flow* category

![Reusable Custom Actions](/assets/images/tutorial-custom-action-2.png){: width="800px" }

Drag and drop the newly created custom action to the flow. 

Apply the `input` and `output` value of the custom actions.  In the below example, we are taking the HTTP `request body` in the custom action `input` and putting the custom actions' `output` into the HTTP `response body`.

![Reusable Custom Actions](/assets/images/tutorial-custom-action-3.png){: width="800px" }


## 2\. Copy Configuration

Select the action you want to copy.  By pressing the copy icon, the configuration for the action gets copied

![Reusable Custom Actions](/assets/images/tutorial-copy.png){: width="600px" }

## 3\. Paste Configuration

Select the paste icon.
![Reusable Custom Actions](/assets/images/tutorial-paste.png){: width="600px" }

A paste pop-up will appear.  If you already copied an action, the pop-up will auto-populate.

If you are copying the configuration from another source, simply paste the configuration in the input box and press [OK].

![Reusable Custom Actions](/assets/images/tutorial-paste-1.png){: width="500px" }

### Copy and Paste Shortcut

On the MAC, press `Alt` + drag and drop the action.



## 4\. Upload and Export Configuration

Go to the **Settings** section.

### Download Configuration

Press the **Download** button to save the configuration on your computer. The default file name is `config.json`.

![Download configuration](/assets/images/tutorial-config-download.png){: width="700px" }

### Upload Configuration

Press the **Upload** button to save the configuration on your computer. 

![Upload configuration](/assets/images/tutorial-config-upload.png){: width="800px" }

You can choose the parts you want to upload by selecting the checkboxes.

![Upload configuration](/assets/images/tutorial-config-upload-1.png){: width="800px" }


## 5\. Rollback

The rollback on your changes by pressing the **Undo** button.  The rollback will take you solution back to when the last change was made.

![Change History](/assets/images/tutorial-change-history.png){: width="800px" }


## 6\. Organizing Actions

Go to the **Organization** category to use the **Group** action.

![Organizing Actions](/assets/images/tutorial-organizing-actions.png){: width="800px" }

Drag and drop the actions in the **Group**. Users can copy, move, and delete the entire group in a single action.

![Organizing Actions](/assets/images/tutorial-organizing-actions-1.png){: width="600px" }

## 7\. Organizing Endpoints

### Creating the Endpoint Group
Select the **Server** for the endpoints to group.  Create a new group by pressing the `+` button next to Endpoint Groups.

![Organizing Endpoints](/assets/images/tutorial-organizing-endpoints.png){: width="600px" }

### Adding Endpoints
Press the **Endpoint** that you wish to group.  Select the group name from the dropdown.

![Organizing Endpoints](/assets/images/tutorial-organizing-endpoints-1.png){: width="600px" }

The endpoints can be grouped for easier organization and visualization.

![Organizing Endpoints](/assets/images/tutorial-organizing-endpoints-3.png){: width="500px" }

### Deleting Endpoint Group

From the server settings, click the `group name` to delete the group.

![Organizing Endpoints](/assets/images/tutorial-organizing-endpoints-4.png){: width="500px" }


<!-- {% include in_line_banner_config.html config_title="Organization" config_url="/assets/configs/_____.json" %} -->


[NEXT >> Lesson 11: Scheduling Flow Execution Using Timers](/docs/tutorial-video/course-basics/lesson-timers/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

{: .fs-6 .fw-300 }
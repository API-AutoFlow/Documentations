---
layout: default
title: Configure API Autoflow
parent: Internal Actions
has_children: true
permalink: /docs/internal-actions/config-autoflow
---
**Install version only**


|                  | Purpose                       |
|:-----------------|:------------------------------|
| **Create Timer** | Used to create a new timer dynamically. It will execute a configured flow at a configured interval. Its output includes the timer ID. |
| **Update Timer** | Used to update timer’s configuration such as interval, and flow being executed. Timer ID is used to target the correct timer. |
| **Get Timer** | Used to get timer information for the targeted timer-id. There is a fixed issue with this action that will be included in the next release. |
| **Delete Timer** | Used to delete a timer with targeted timer-id. Currently, delete timer action deletes a timer with the targeted timer-id. However, the UI does not refresh the delete. UI refresh will show the correct state of timer configuration. There is an open issue to fix this UI issue. |
| **Start Timer** | Used to start a timer with targeted timer-id.  |
| **Stop Timer** | Used to stop a timer with targeted timer-id. |
| **Get ID** |  |
| **Get Resources** |  |


## Sample Configuration
Click to [learn how to upload configuration](https://docs.apiautoflow.com/docs/tutorial-video/course-1-basics/lesson-10-organization/#paste-configuration) into your solution.

### [Download Configuration](https://docs.apiautoflow.com/assets/configs/config-autoflow-timer.json)


{: .fs-6 .fw-300 }

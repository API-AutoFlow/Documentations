---
layout: default
nav_order: 11
title: Lesson 11 Timers
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 10 min video
<h1 style="margin-top:0">Lesson 11: Scheduling Flow Execution Using Timers</h1>

Timers are used to schedule triggered events at a set interval.

## Lesson Outline

1. Create Timer
2. Apply action(s) to the Timer
3. Apply action(s) to the Timer
4. Control Timer


## 1\. Create Timer

Create a new timer by selecting **Timer** from the drop-down.

![Timer](/assets/images/tutorial-timer.png){: width="400px" }


## 2\. Set Timer

Set the timer to the desired interval.  The time is in `milliseconds`.

![Timer](/assets/images/tutorial-timer-1.png){: width="600px" }

## 3\. Apply action(s) to the Timer

Apply actions to the timer's flow.  A common use case is to trigger a flow using a timer.
![Timer](/assets/images/tutorial-timer-2.png){: width="500px" }

## 4\. Control Timer

There are use cases where timers need to be stopped and started based on a condition.  Use the [config/timer](/docs/internal-actions/config-autoflow/timer-create/) actions to automate the timer.

![Timer](/assets/images/tutorial-timer-3.png){: width="700px" }


{% include in_line_banner_config.html config_title="Scheduling Flow Execution Using Timers" config_url="/assets/configs/config-timer.json" %}


[NEXT >> Lesson 12: Debugging Using Logs](/docs/tutorial-video/course-basics/lesson-debug/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }

{: .fs-6 .fw-300 }
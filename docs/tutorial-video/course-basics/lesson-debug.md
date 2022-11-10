---
layout: default
nav_order: 12
title: Lesson 12 Debugging
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 6 min video
<h1 style="margin-top:0">Lesson 12: Debugging Using Logs</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/RTvW8qRFMII" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Lesson Outline

1. Action Error
2. Apply Data/Log Action

## 1\. Action Error

When an error occurs with an action, the action is alerted in <span style="color:red">**RED**</span>.

In the below example, the action **integer to string** is expecting an `integer` but got a string value of `Hello World`.

<span style="color:red">*Expected Integer for "integer" but received non-integer value: "Hello World"*</span>

![Debugging](/assets/images/tutorial-debug.png){: width="700px" }

## 2\. Apply Data/Log Action

In most cases debugging happens with simulated data. That is because flows are made to handle the input data and generate the desired output.

Apply [data/log](/docs/internal-actions/data/log/) action anywhere in the flow to print the data.

In the example below, note that two [data/log](/docs/internal-actions/data/log/) actions are applied.

* The first `data/log 1` log the data and shows `hello`.
* The second `data/log 2` log the data after the [string/upcase](/docs/internal-actions/string/upcase/) has been applied and shows `HELLO`.

![Debugging](/assets/images/tutorial-debug-1.png){: width="800px" }

Note that the data printed is what the [data/log](/docs/internal-actions/data/log/) action received where it is applied.

{% include in_line_banner_config.html config_title="Debugging Using Logs" config_url="/assets/configs/config-debug.json" %}

[NEXT >> Course 2: Advanced](/docs/tutorial-video/course-solutions/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


{: .fs-6 .fw-300 }
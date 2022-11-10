---
layout: default
nav_order: 7
title: Lesson 7 API Calls
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 4 min video
<h1 style="margin-top:0">Lesson 7: Making API Calls</h1>

<iframe width="560" height="315" src="https://www.youtube.com/embed/I9adsQtrWDc" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Lesson Outline

1. Apply Communication/HTTP-Request action
2. Fill in the API Details
3. Check the API Response

## 1\. Apply Communication/HTTP-Request action

From the `right navigation`, select the `communication` category. 

![Apply HTTP Request Action](/assets/images/tutorial-http.png)

Drag and drop the [HTTP request](/docs/external-actions/communication/http-request/) condition to the flow

![Apply HTTP Request Action](/assets/images/tutorial-http-1.png)

## 2\. Fill in the API Details

A postman echo API will be used to test the API request.

URL: `https://postman-echo.com/get?foo1=bar1&foo2=bar2` <br />
Method: GET

For more information, click [postman echo](https://www.postman.com/postman/workspace/published-postman-templates/documentation/631643-f695cab7-6878-eb55-7943-ad88e1ccfd65?ctx=documentation)

Set the output to `result`

![Apply HTTP Request Action](/assets/images/tutorial-http-2.png){: width="600px" }

## 3\. Check the API Response

In the `flow transaction data`, the API successfully got the data from the API.

![Apply HTTP Request Action](/assets/images/tutorial-http-3.png){: width="800px" }

## 4\. Other HTTP Requests

There are many types of HTTP API. Check the API provider's manual for the correct HTTP action to use.

![Apply HTTP Request Action](/assets/images/tutorial-http-4.png){: width="400px" }


{% include in_line_banner_config.html config_title="Making API Calls" config_url="/assets/configs/config-httprequest.json" %}

[NEXT >> Lesson 8:  In Memory Storage - Hash Table](/docs/tutorial-video/course-basics/lesson-inmemory/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


{: .fs-6 .fw-300 }
---
layout: default
nav_order: 4
title: Lesson 4 Conditions
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 5 min video
<h1 style="margin-top:0">Lesson 4: Build Your First Flow Using Conditionals</h1>

Now that you have a good grasp of the fundamentals, let's look at how to create more complex solutions.

The conditionals are statements like **IF, Match, the Switch** that perform a set of actions when the conditions are met.

<iframe width="560" height="315" src="https://www.youtube.com/embed/6cgOFMzWhfk" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

If you had any interest in technology, I am sure you have come across the **"IF"** condition (no pun intended).

**"Match"** is similar in a way that instead of `true` or `else`, it has a list of conditions.

## Lesson Outline

1. Apply `Conditional` action to the `flow`
2. Set condition rule
3. Apply actions to the conditions

## 1\. Apply `Conditional` action to the `flow`

From the `right navigation`, select the `conditional` category. 

![Action Conditional Select](/assets/images/action-if-condition-select.png)

Drag and drop the `IF` condition to the flow

![Action Conditional Select](/assets/images/action-if-condition-select-0.png)

## 2\. Set condition rule

Select the **`IF`** action and use the drop-down to set the condition.

In the below example, we are selecting the `string/contains` a condition. **String/contains** checks whether the `target` contains a certain `string` value.

![Action Conditional Select](/assets/images/action-if-condition-select-1.png)

Let's set the target as `request/body`.

![Action Conditional Select](/assets/images/action-if-condition-select-2.png)

If the target `request/body` contains a `string` value **"Hello"**, the condition is `true`, otherwise, it is `else`.

To test the solution, you can use the `flow test simulation` to mock the `request/body`.

![Action Conditional Select](/assets/images/action-if-condition-select-3.png)

## 3\. Apply actions to the conditions

In the `true` part of the **IF** condition, apply the `data/set` action.

* Make the value **"True"**
* Make the output as **"response/body"**

You will notice that since the condition is true, it will execute the action "data/set" to return the value "True"

![Action Conditional Select](/assets/images/action-if-condition-select-4.png)

{% include in_line_banner_config.html config_title="Build Your First Flow Using Conditionals" config_url="/assets/configs/config-course1-lesson4-conditional.json" %}

[NEXT >> Lesson 5: Master Loops(Iterations) to Create Complex Solutions](/docs/tutorial-video/course-1-basics/lesson-5-iterations/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


{: .fs-6 .fw-300 }
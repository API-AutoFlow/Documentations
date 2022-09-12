---
layout: default
title: Lesson 4 Conditions
parent: Course 1 Getting Started
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
<h1 style="margin-top:0">Lesson 4: Build Your First Flow Using Conditionals</h1>

Now that you have a good grasp of the fundamentals, let's look at how to create more complex solutions.

<iframe width="560" height="315" src="https://www.youtube.com/embed/jKihyMvokiA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

The conditionals are statements like **IF, Match, Swith** that performs a set of actions ("`flow`") when the condition matches.

If you had any interest in technology, I am sure you have come across **"IF"** condition (no pun intended).

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

In below example, we are selecting the `string/contains` condition. **String/contains** checks whether the `target` contains a certain `string` value.

![Action Conditional Select](/assets/images/action-if-condition-select-1.png)

Let's set the target as `request/body`.

![Action Conditional Select](/assets/images/action-if-condition-select-2.png)

If the target `request/body` contains `string` value **"Hello"**, the condition is `true`, otherwise it is `else`.

To test the solution, you can use the `flow test simulation` to mock `request/body`.

![Action Conditional Select](/assets/images/action-if-condition-select-3.png)

## 3\. Apply actions to the conditions

In the `true` part of the **IF** condition, apply the `data/set` action.

* Make the value as **"True"**
* Make the output as **"response/body"**

You will notice that since the condition is true, it will execute the action "data/set" to return the value "True"

![Action Conditional Select](/assets/images/action-if-condition-select-4.png)






[NEXT >> Lesson 5: Master Loops(Iterations) to Create Complex Solutions](/docs/tutorial-video/course-1-basics/lesson-5-master-loops-iterations-to-create-complex-solutions/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


{: .fs-6 .fw-300 }
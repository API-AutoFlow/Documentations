---
layout: default
nav_order: 5
title: Lesson 5 Iterations
parent: Course 1 Basics
grand_parent: Tutorials - Video
published: true
---
<h6>Course 1: Getting started with API AutoFlow</h6>
2 min read · 8 min video
<h1 style="margin-top:0">Lesson 5: Master Iteration (loop) to Create Complex Solutions</h1>

Once you have a good understanding of **loops**, you can build a wide range of solutions.

The good news is that loops are relatively easy to understand. There are just a few things that you need to remember

1. Loop iterates over a list (array)
2. You apply actions to each item on the list

So, if you want to apply the same action to each item on the list, it helps to have all the items to be in the same format (a.k.a structured data).

<iframe width="560" height="315" src="https://www.youtube.com/embed/kE3yWUW_060" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Lesson Outline

1. Apply `Interation` action to the `flow`
2. Set the array to loop over
3. Apply actions to the conditions


## 1\. Apply `Interation` action to the `flow`

From the right navigation, select the [iteration](/docs/internal-actions/iteration/) category.

![Action Conditional Select](/assets/images/action-loop-1.png)

Drag and drop the [filter](/docs/internal-actions/iteration/filter/) iteration to the flow.  

The [filter](/docs/internal-actions/iteration/filter/) iteration only passes value when `true`.  So, inside the iteration, we will need to put a `boolean` condition to filter our `result`.

![Action Conditional Select](/assets/images/action-loop-2.png)

### Simulation data

To help with the solution building, let's simulate an array with `["name", "gender"]`.  We will create an iteration to filter just `female`.

[Click here to learn more about data simulation](/docs/tutorial-video/course-basics/lesson-data-sumulation/)

![Action Conditional Select](/assets/images/action-loop-data-simulation.png)

## 2\. Set the array to loop over

Drag and drop the `request/body` that we just simulated to the iteration action.

![Action Conditional Select](/assets/images/action-loop-3.png)

### Understanding output

To apply actions on items, it helps to reference the `index` and the `value` of the iterated items.
The final output is the `result`.

Note. The `filter` iteration action only passed when the **value** is `1` (true).

So, as the iteration goes over each of the items, we need to make the value into `1` to add it in the final `result`

![Action Conditional Select](/assets/images/action-loop-4.png)


## 3\. Apply action to the conditions

The condition can look for the word `female`.  There's perfect action for that called [string/contain](/docs/internal-actions/string/contains/).

String/contains action checks if the data contains a certain string and output `1` for true and `0` for false.

![Action Conditional Select](/assets/images/action-loop-5.png)

Drag-and-drop the [string/contain](/docs/internal-actions/string/contains/) action inside the iteration.

![Action Conditional Select](/assets/images/action-loop-6.png)

Again, the iteration checks the `value` of each item from the array. In the right bottom pane, you have access to the `value`.

Note: Only the **first value** from the array is shown for reference.

Drag-and-drop the `value` to the action's properties.

![Action Conditional Select](/assets/images/action-loop-7.png)

Next input the content that we want to filter. In our case, we are looking for items with the string `"female"`.

Output needs to be `value` since the iteration looks at the value for true or false.

![Action Conditional Select](/assets/images/action-loop-8.png){: width="500px" }

Click on the small square outside the iteration.  After the iteration is complete, it will output `result` with the value `1` (true).

Below, we have filtered the items with string `female`.

![Action Conditional Select](/assets/images/action-loop-9.png)

{% include in_line_banner_config.html config_title="Master Iteration (loop) to Create Complex Solutions" config_url="/assets/configs/config-iteration.json" %}

[NEXT >> Lesson 6: Learn How to Work with Databases and APIs](/docs/tutorial-video/course-basics/lesson-databases/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }


{: .fs-6 .fw-300 }
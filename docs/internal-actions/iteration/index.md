---
layout: default
title: Iteration
parent: Internal Actions
has_children: true
permalink: /docs/internal-actions/iteration
---

The `iteration` actions are like `loop` in programing language.
It iterates over each `value` in the `array` and executes flow of actions that are place inside.

When configuring `iterations`, you are have to work with `index` and `value` of the array.  When you turn on the `dev mode`, you have access to the first(index 0) value from the array as a sample to work with.

There are many types of `iteration` actions to choose from. Below is a table of their purpose, pros, and cons
 

|                  | Purpose                       | Pros                       | Cons                                         |
|:-----------------|:------------------------------|:---------------------------|:---------------------------------------------|
| **All are True** | Tests array to see if all are true |  Fast  | Does not extract value, Does not change data |
| **Any is True**  | Tests array to see if any is true |     Fast      |  Does not extract value, Does not change data |
| **Filter**       | Filter elements               | Fast                       | Does not extract value, Does not change data |
| **Find Index**   |  |    |  |
| **Find Value**   |    |           |                                   |
| **Find**         |  |    |  |
| **For Each**     | Extract value & take action   | Can extract value          | Can be slow                                  |
| **Map**          | Apply change to original data | Can change original Data   | Does not extract value, Does not filter data |
| **While**        |               |                        |  |


{: .fs-6 .fw-300 }

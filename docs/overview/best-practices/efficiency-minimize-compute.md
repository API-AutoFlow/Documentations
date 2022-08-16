---
layout: default
title: Efficiency Minimize compute processing
parent: Best Practices
grand_parent: Overview
---

# Efficiency: Minimize compute processing
There are actions that use more compute than others.  A general rule of thumb is to think of how much data processing the action has to perform.

For example, a common data extraction use case of iterating over a list, selecting the value from each element, and inserting it into a new list.

* Process 1: Iteration/for-each takes each element and saves it in the memory
* Process 2: Array-insert breaks down the data, selects the value, and insert it into the array

If there are thousands of elements in the list, you can imagine the compute needed to save each element in memory and break them for processing. Instead, using Boolean actions such as iteration/filter that checks if the element is true or false and throws away the non-matching element is more efficient.

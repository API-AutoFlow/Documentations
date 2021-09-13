---
layout: default
title: Iteration Map
parent: Iteration
grand_parent: Actions
---
# Iteration Map
MAP iterates over the array and replaces the value.  Hence actions that change the value are commonly used inside the Iteration Map action.

## Properties
```yaml
Array:  The location of the array that’s been iterated over
```

## Output
```yaml
Index-location: The location to store each index
Value-location: The location to store email value
Output-location: The location the original array is stored
```

### Example
Let’s say we want to iterate over an array [“a”, “b”, “c”] and capitalize each value.

1. Using the Testing feature, let’s send an array of [“a”, “b”, “c”] in the request body
2. Add an Iteration Map Action and assign where you want to read the array from (list-target) and where you want to put the resulting value (value-target)
3. The action that we want to iterate is first to capitalize the letters, so we will use the action String Capitalize
4. Finally, we need to set the data in the response body to visualize it on the browser.  Let’s read from the data element “iterate” and put it in the “response body”

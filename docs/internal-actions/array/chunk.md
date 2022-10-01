---
layout: default
title: Chunk
parent: Array
grand_parent: Internal Actions
---
# Array Chunk
Returns list of lists containing count elements each, where each new chunk starts step elements into the enumerable.

## Properties
```yaml
Array: Location of the list to chunk
Count: The number of elements for the new chunk (list)
Step: The steps into the enumerable each new chunk starts
Leftover: The value to fill the last chunk if not completely filled
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Let’s say we have a list with six elements.

Target: Location of the original list
```js
[1, 2, 3, 4, 5, 6]
```
Group the chunk in elements of three.

Count: `3`

The start of each chunk to start two steps into the enumerable

Step: `2`

If the last chunk is not completely filled, include this value to the end.

Leftover: `7`

**Result**
```js
[[1, 2, 3], [3, 4, 5], [5, 6, 7]]
```

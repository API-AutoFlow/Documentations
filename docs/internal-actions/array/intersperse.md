---
layout: default
title: Array Intersperse
parent: Array
grand_parent: Internal Actions
---
# Array Intersperse
Inserts separator between the elements of the list.

## Properties
```yaml
Array: Location of the list to add the value
Element: The value to add between the elements
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Let’s say we have below a list
```js
[a, b, c]
```
And the separator ‘d’ is inserted

Element: `d`

**Result**
```js
[a, d, b, d, c]
```

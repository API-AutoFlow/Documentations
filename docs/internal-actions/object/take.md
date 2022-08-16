---
layout: default
title: Object Take
parent: Object
grand_parent: Internal Actions
---
# Object Take (Extracts key-value pair into a new object)
Returns a new map with all the key-value pairs in map where the key is in keys.

## Properties
```yaml
Object: Location of the object to take the value from
Keys: Key of the value to extract
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
From the object
```js
{a: 1, b: 2, c: 3}
```
extract values matching the keys
```js
[a, c, e]
```

This will return
```js
{a: 1, c: 3}
```

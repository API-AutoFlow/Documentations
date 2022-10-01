---
layout: default
title: Split
parent: String
grand_parent: Internal Actions
---
# String Split (Split the string into array)
Divides a string into substrings at each Unicode whitespace occurrence with leading and trailing whitespace ignored. Groups of whitespace are treated as a single occurrence. Divisions do not occur on non-breaking whitespace.

## Properties
```yaml
String: Location of the string to split
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Applying the String Split action to the string `“foo bar”` will return
```js
[“foo”, “bar”]
```

---
layout: default
title: Wrap
parent: Array
grand_parent: Internal Actions
---
# Array Wrap
Wraps term in a list if this is not listed.
If term is already a list, it returns the list. If term is nil, it returns an empty list.

## Properties
```yaml
Element: the value to turn into an array
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
* String `“hello”` will output `[“hello”]`
* Array `[1, 2, 3]` will output `[1, 2, 3]`
* `nil` will output `[]`

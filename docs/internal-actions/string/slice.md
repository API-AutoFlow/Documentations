---
layout: default
title: Slice
parent: String
grand_parent: Internal Actions
---
# String Slice (Slices the string)
Returns a substring starting at the offset start, and of given length.

## Properties
```yaml
String: Location of the string to work on
Start: String position to start the slice
Length: The length of the new string
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
From the string `“hello world”`, start at position `“6”` for length of `“5“` will return `“world”`

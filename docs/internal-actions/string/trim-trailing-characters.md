---
layout: default
title: Trim Trailing Characters
parent: String
grand_parent: Internal Actions
---
# String Trim Trailing Characters
Returns a string where all trailing to_trim characters have been removed.

## Properties
```yaml
String: Location of the string to trim
Characters: Character to remove from the back of the string
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Trimming a string `“_ abc __”` with the character `“_”` would return `” _ abc “`

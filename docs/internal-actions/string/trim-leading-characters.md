---
layout: default
title: String Trim Leading Characters
parent: String
grand_parent: Internal Actions
---
# String Trim Leading Characters
Returns a string where all leading to_trim characters have been removed.

## Properties
```yaml
String: Location of the string to trim
Characters: Character to remove from front and back of the string
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Trimming a string `“__ abc _”` with the character `“_”` would return `” abc _”`

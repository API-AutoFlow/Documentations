---
layout: default
title: Replace Prefix
parent: String
grand_parent: Internal Actions
---
# String Replace Prefix (Replaces prefix with characters)
Replaces prefix in string by replacement if it matches.

## Properties
```yaml
String: Location of the string to work on
Match: The pattern to look for in the string
Replacement: Value to replace with
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
From the string `“hello hello world”` with pattern of `“hello ”` and replacement `""` will return `“hello world”`

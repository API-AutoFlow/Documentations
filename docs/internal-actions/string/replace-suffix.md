---
layout: default
title: Replace Suffix
parent: String
grand_parent: Internal Actions
---
# String Replace Suffix (Replaces the suffix with the characters)
Replaces suffix in string by replacement if it matches match.

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
From the string `“hello world world”` with pattern of `“_world”` and replacement `“_universe“` will return `“hello world universe”`

---
layout: default
title: Replace Leading
parent: String
grand_parent: Internal Actions
---
# String Replace Leading (Replaces the leading character)
Replaces all leading occurrences of the match by replacement of match in the string. Returns the string untouched if there are no occurrences.

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
From the string `“hello hello world”` with pattern of `“hello ”` and replacement `“ “` will return `“world”`

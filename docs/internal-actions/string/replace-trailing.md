---
layout: default
title: Replace Trailing
parent: String
grand_parent: Internal Actions
---
# String Replace Trailing (Replaces trailing characters)
Replaces all trailing occurrences of match by replacement in string.

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
From the string `“hello world world”` with pattern of `“_world”` and replacement `“_universe“` will return `“hello universe universe”`

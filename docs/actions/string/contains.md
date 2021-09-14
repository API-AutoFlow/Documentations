---
layout: default
title: String Contains
parent: String
grand_parent: Actions
---
# String Contains (Checks if strings contains a given string)
Checks if string contains any of the given contents.

## Properties
```yaml
String: Location of the string
Contents: Content to make the comparison with
```

## Output
```yaml
Output-location: Location to store the output data
```

Contents can be either a string, a list of strings, or a compiled pattern.

### Example
Check whether the string `‘Hello World’` contains the content `‘Hello’` would return `‘true’`

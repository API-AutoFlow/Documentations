---
layout: default
title: Regex is Match
parent: String
grand_parent: Internal Actions
---
# String Regex is Match
Checks if string matches the given regular expression.

## Properties
```yaml
String: Location of the string to match against
Regex: Regex expression to compare
```

Output
```yaml
Output-location: Location to store the output data
```

## Example
A string `foo` matching again regex expresson `~r/foo/` would return **TRUE**

A string `bar` matching again regex expresson `~r/foo/` would return **FALSE**

---
layout: default
title: At
parent: String
grand_parent: Internal Actions
---
# String At (Get character at nth position)
Retrieves the character at the nth position.

Returns the grapheme at the position of the given UTF-8 string. If position is greater than string length, then it returns nil.

## Properties
```yaml
String: Location of the string to retrieve the character from
At: Position of the character to retrieve (Position starts from 0)
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Retrieving character from position `3` of string `Interactor` would return `r`

---
layout: default
title: JSON Decode
parent: JSON
grand_parent: Internal Actions
---
# JSON Decode
Parses a string as a subset of YAML, and produces a representation of its value.

## Properties
```yaml
YMAL: Location of the YMAL
```

## Output
```yaml
Output-location: The location to store the output data
```

### Example
A string value of

```js
"{a: [1, 2, 3], b: foo}"
```
will parse to
```js
{
  "a" = [
    1,
    2,
    3,
  ]
  "b" = “foo”
}
```

---
layout: default
title: JSON Encode
parent: JSON
grand_parent: Internal Actions
---
# JSON Encode
Encodes a given value to a string using YAML 1.2 block syntax.

## Properties
```yaml
Data: Location of the data
```

## Output
```yaml
Output-location: The location to store the output data
```

### Example
Below data will be encoded
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
into output of
```js
"{a: [1, 2, 3], b: foo}"
```

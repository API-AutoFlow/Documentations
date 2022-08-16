---
layout: default
title: Float Floor
parent: Float
grand_parent: Internal Actions
---
# Float Floor
Rounds a float down to the largest integer less than or equal to the number. Precision is the decimal place.

## Properties
```yaml
Float: Location of the number to round
Precision: Precision of the decimal place
```
E.g ‘1’for rounding to the tenths decimal

## Output
```yaml
Output-location: Location to store the output data
```

### Example
`1.17` will become `1.16` if the precision is set to `2` decimal place

---
layout: default
title: Integer Undigits
parent: Integer
grand_parent: Internal Actions
---
# Integer Undigits (Undigits from Array)
Returns the integer represented by the ordered digits.  An optional base value may be provided representing the radix for the digits.

## Properties
```yaml
Array: Location of the array to undigit
Base: Digit base E.g. Digit ‘2’ will convert the integer into binary
```

## Output
```yaml
Output-location: Location to store the output data
```

### For example
A list `[1, 2, 3]` with base `0` will return `123`

A list `[1, 4]` with base `16` will return `20`

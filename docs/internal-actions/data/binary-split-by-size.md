---
layout: default
title: Binary Split by Size
parent: Data
grand_parent: Internal Actions
---
# Binary Split by Size

Split binary data by size.

## Properties
```yaml
value: The value to split
size: Split by size
```

## Output
```yaml
output-location: Location to store the output data
```

## Example configuration

```yaml
value: ABCDE
size: 2
```

## Example output

```yaml
[
  "AB",
  "CD",
  "E"
]
```
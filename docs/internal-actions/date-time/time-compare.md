---
layout: default
title: Time Compare
parent: Date Time
grand_parent: Internal Actions
---
# Time Compare
Check if two Time are equal..  

Date and Time format
```js
HH:MM:SS
```
with – date = output.   Where “0” is true and “1” is false

## Properties
```yaml
Date: Location of the first time
With: The second time to check against
```

## Output
```yaml
Output-location: The location to store the output
```

## Example
date: `12:03:12`

with: `11:23:34`

output: `1` (FALSE)

---
layout: default
title: Date and Time Compare
parent: Date Time
grand_parent: Internal Actions
---
# Date and Time Compare
Check if two date + Time are equal..  

Date and Time format
```js
YYYY-MM-DDThh:mm:ss.sTZD
```
(eg 1997-07-16T19:20:30.45+01:00)
with – date = output.   Where “0” is true and “1” is false

## Properties
```yaml
Date: Location of the first date and time
With: The second date and time to check against
```

## Output
```yaml
Output-location: The location to store the output
```

Example
date: `2002-02-02T19:20:30.45+01:00`

with: `2002-02-01T19:22:30.45+01:00`

output: `1` (FALSE)

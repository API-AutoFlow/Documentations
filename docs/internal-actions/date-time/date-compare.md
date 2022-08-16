---
layout: default
title: Date Compare
parent: Date Time
grand_parent: Internal Actions
---
# Date Compare
Check if two dates are equal..  

Date format
```js
YYYY-MM-DD
```
with – date = output.   Where “0” is true and “1” is false

## Properties
```yaml
Date: Location of the first date
With: The second date to check against
```

## Output
```yaml
Output-location: The location to store the output
```

Example
date: `2002-02-02`

with: `2002-02-01`

output: `1` (FALSE)

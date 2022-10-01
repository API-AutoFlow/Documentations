---
layout: default
title: URI URL encode
parent: String
grand_parent: Internal Actions
---
# String URI URL encode (Encodes String as “x-www-form-urlencoded”)
String URI URL Encode. Encodes string as “x-www-form-urlencoded”.

## Properties
```yaml
String: Location of the string to encode
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
URL of `“put: it+й”` will return `” put%3A+it%2B%D0%B9″`

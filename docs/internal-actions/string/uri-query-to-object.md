---
layout: default
title: URI Query to Object
parent: String
grand_parent: Internal Actions
---
# String URI Query to Object
Returns a stream of two-element tuples representing key-value pairs in the given query.

## Properties
```yaml
String: Location of the query string to decode into an object
```

## Output
```yaml
Output-location: Location to store the output data
```

Key and value in each tuple will be binaries and will be percent-unescaped.

### Example
URI query of `“(“foo=1&bar=2”) |> Enum.to_list()”` will return `“[{“foo”, “1”}, {“bar”, “2”}]”`

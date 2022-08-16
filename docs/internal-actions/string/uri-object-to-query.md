---
layout: default
title: String URI Object to Query
parent: String
grand_parent: Internal Actions
---
# String URI Object to Query
Encodes an enumerable into a query string.

## Properties
```yaml
Object: Location of the enumerable to encode into a query string
```

## Output
```yaml
Output-location: Location to store the output data
```

Takes an enumerable that enumerates as a list of two-element objects (for instance, a map or a keyword list) and returns a string in the form of key1=value1&key2=value2… where keys and values are URL encoded as per encode_www_form/1.

### Example
URI query of `“{“key” => “value with spaces”}”` will return `“key=value+with+spaces”`

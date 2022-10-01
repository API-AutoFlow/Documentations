---
layout: default
title: URI Percent Encode
parent: String
grand_parent: Internal Actions
---
# String URI Percent Encode (Percentage Escape All Characters)
URI Percent Encode. Percent-escapes all characters that require escaping in string.

## Properties
```yaml
String: Location of the URI to encode
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
Decoding to the URI `” ftp://s-ite.tld/?value=put it+й”` will return `”ftp://s-ite.tld/?value=put%20it+%D0%B9″`

---
layout: default
title: Data Parse
parent: Data
grand_parent: Internal Actions
---
# Data Parse
Parse binary data using a binary schema. If target packet is not provided, it tries to match any packet type in a given schema.

## Properties
```yaml
Value: Location of the value to check      
schema-id: Binary Schema to use for parsing given value
target: Target binary packet type to parse against
value: The value to parse
```

## Output
```yaml
Output-location: Location to store the output data
```

## Sample Configuraiton

How to apply sample configuration to API AutoFlow.

```yaml
{
  "info": {},
  "packets": {
    "packet1": {
      "fields": [
        {
          "filler": "0",
          "name": "packet_length",
          "size": 4,
          "size_unit": "byte",
          "type": "packet_length",
          "value_type": "string"
        },
        {
          "filler": "0",
          "name": "packet_type",
          "size": 4,
          "size_unit": "byte",
          "value_type": "string"
        }
      ]
    }
  }
}
```

### Example value
`0004TEST`

### Example parsed object output
```yaml
{
  "matched": "packet1",
  "parsed": {
    "packet_length": "0004",
    "packet_type": "TEST"
  },
  "status": "success"
}
```
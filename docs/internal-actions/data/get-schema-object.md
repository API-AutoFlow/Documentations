---
layout: default
title: Get Schema Object
parent: Data
grand_parent: Internal Actions
---
# Get Schema Object
Gets binary schema structure object for a given `schema` and `target packet`

## Properties
```yaml
Schema ID: Location or value of binary schema. Schema-id can be selected from drop down, or dynamically referenced by saving the Schema-id at the time of creation.
Target: Location or value of target parcket within the binary schema
```

## Output
```yaml
output-location: Location to store the output data
```

## Example binary schema configuration

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

## Example binary schema object output
```yaml
{
  "status": "",
  "value-object": {
    "packet_length": "",
    "packet_type": ""
  }
}
```
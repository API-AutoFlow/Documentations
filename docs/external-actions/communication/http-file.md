---
layout: default
title: Communication HTTP File Request
parent: Communication
grand_parent: External Actions
---

# Communication HTTP File Request

Make HTTP file request.

## Properties
```yaml
url: Address for the Request to be sent
path: Path of the request. You can use "{variable-name}" syntax to create variable placeholders
url-variables: variable url path values in an object of key value pairs
filepath: path of file to send
keyname: form data name to use
filename: form data filename to use
header: Value to include in the header
query: Query to the server
timeout: Duration to make attempt
```

## Output
```yaml
output-location: Location to store the output data
```
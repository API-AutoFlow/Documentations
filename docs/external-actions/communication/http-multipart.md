---
layout: default
title: HTTP Multipart
parent: Communication
grand_parent: External Actions
---

# Communication HTTP Multipart Request

Make HTTP multipart request.

## Properties
```yaml
url: Address for the Request to be sent
path: Path of the request. You can use "{variable-name}" syntax to create variable placeholders
url-variables: variable url path values in an object of key value pairs
type: type of HTTP request to use for sending form data
multipart: list of part objects with keys
type: form or file
key: part key if of type form
value: part value if of type form
filepath: part filepath if of type file
keyname: part keyname if of type file. Defaults to "uploaded_file"
filename: part filename if of type file. Defaults to filename from basename of filepath
header: Value to include in the header
query: Query to the server
timeout: Duration to make attempt
```

## Output
```yaml
output-location: Location to store the output data
```
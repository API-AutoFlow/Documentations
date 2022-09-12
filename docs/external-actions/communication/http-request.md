---
layout: default
title: HTTP Request
parent: Communication
grand_parent: External Actions
---

# HTTP Request
Makes HTTP request to APIs from the flow.

## Properties
```yaml
url: Address for the Request to be sent
path: Path of the request. You can use "{variable-name}" syntax to create variable placeholders
url-variables: variable url path values in an object of key value pairs
method: Refer to Endpoint for more information
body: Value to include in the body
Header: Value to include in the header
Query: Query to the server
Timeout:  Duration to make the attempt
```
## Output
```yaml
Output-location: Location to store the output data
```
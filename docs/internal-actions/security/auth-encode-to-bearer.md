---
layout: default
title: Authentication Encode Basic
parent: Security
grand_parent: Internal Actions
---
# Authentication Encode Basic
Adds the word “Bearer” to the token

## Properties
```yaml
Token: token to be used
```

## Output
```yaml
Output-location: Location to store the output data
```

### Example
**token** of eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9

generates an output of
```
Bearer eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9
```

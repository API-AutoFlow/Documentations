---
layout: default
title: Rest Connector
parent: AWS
grand_parent: Services
---
# AWS Rest based API Connector
API AutoFlow built-in AWS connectors using REST method.
Refer to the AWS documentation to see whether the API endpoint you wish to use supports JSON, Query, or Rest.  
AWS API connectors are also available in the Connectors section.

## Properties
```yaml
Service: Select the AWS service
Method: Select the method (GET, PUT, POST, etc)
Headers: Add the header as per the AWS API documentation
Path: Add the path of the AWS API endpoint to use
Data: Add the data as per the AWS API documentation
Region: Select the region for your server
Access-key-id: Enter the access-key created from AWS IAM
Secret-access-key: Enter the access-key created from AWS IAM
```

## Output
```yaml
Output-location: Location to store the output data
```

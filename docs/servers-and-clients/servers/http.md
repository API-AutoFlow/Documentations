---
layout: default
title: HTTP
parent: Servers
grand_parent: Servers and Clients
---
# HTTP Server

## Port Number
A number representing a communication endpoint.
There are 65,535 port numbers to choose from.

## Base path
A prefix to apply to every path.
A Base Path + Endpoint Path = Full Path
For example

```
/api/v1 + /resouce = /api/v1/resource
```

## TLS
Formerly known as SSL, TLS is an encryption protocol used to enable HTTPS service

## Access Control
Response header indicates whether the response can be shared with requesting code from the given method, origin, and header


![HTTP](/assets/images/server-http.png)


<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

## Reserved port numbers
There are reserved port numbers that can not be used. Refer to commonly made mistakes for details.

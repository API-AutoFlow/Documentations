---
layout: default
title: Security
parent: Definitions
grand_parent: Overview
nav_order: 16
---

# Security
API AutoFlow provides both data security and access control.

## HTTPS TLS (formerly SSL)

Refer to [HTTPS](https://docs.apiautoflow.com/docs/key-concepts/servers/https-tls/) for more detail.

## Data Encryption
API AutoFlow provides data security actions to encrypt and decrypt data.

Refer to [Security Actions](https://docs.apiautoflow.com/docs/internal-actions/security) for more detail.

* Decrypt
* Encrypt
* Hash
* Mac

## Access Control
UserID based access control can be managed from the Administrator section.

Refer to [Administration Section](https://docs.apiautoflow.com/docs/key-concepts/administration-and-settings/) for more detail.

## OWASP Top 10

### A1:2017-Injection
SQL Injection safety in API AutoFlow is supported by underlying library. Solution creators are also encouraged to add additional checks before using user input in SQL queries.

### A2:2017-Broken Authentication
Support for multiple authentication methods is provided to ensure correct implementation of authentication is just a few clicks aways.

### A3:2017-Sensitive Data Exposure
Refer to [Security Actions](https://docs.apiautoflow.com/docs/internal-actions/security) for data security actions

### A4:2017-XML External Entities (XXE)
Support for XML encode/decode is provided as actions. Take care to only allow controlled and known XML documents for processing.

### A5:2017-Broken Access Control
Flexible Access Control may be implemented based on various data sources. Solution creators are encouraged to implement a level of access control right for the solution being created.

### A6:2017-Security Misconfiguration
Empty body is returned by default. Solution creators has control over what gets returned on each request.

### A7:2017-Cross-Site Scripting XSS
Data is not shared between users.

### A8:2017-Insecure Deserialization
There is no default serialization of user data. Solution creators are encouraged to take care when using user data for serialization.

### A9:2017-Using Components with Known Vulnerabilities
External components may not be used with API AutoFlow.

### A10:2017-Insufficient Logging & Monitoring
Refer to [Logging](https://docs.apiautoflow.com/docs/key-concepts/logs/)
Refer to [Data](https://docs.apiautoflow.com/docs/key-concepts/data/)

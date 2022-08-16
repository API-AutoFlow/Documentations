---
layout: default
title: Syslog UDP RFC3164
parent: Communication
grand_parent: External Actions
---

# Syslog UDP RFC3164
RFC3164 is “the old format” of Syslog.

## Properties
```yaml
Message: Syslog message
Address: Destination address. e.g. 127.0.0.1
Port: Destination port
Facility: Syslog facility
Severity: Syslog severity
Hostname: Hostname to be used for the Syslog message
Process-name: A process name to be used for the Syslog message
```

## Output
```yaml
output-location: Location to store the output data
```

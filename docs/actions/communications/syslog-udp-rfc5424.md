---
layout: default
title: Syslog UDP RFC5424
parent: Communications
grand_parent: Actions
---

# Syslog UDP RFC5424
{: .no_toc }

RFC5424 is “the new format” of Syslog.

## Properties
```yaml
Message: Syslog message
Address: Destination address. e.g. 127.0.0.1
Port: Destination port
Facility: Syslog facility
Severity: Syslog severity
Hostname: Hostname to be used
Process-name: A process name to be used
Process-id: Process ID to be used
Message-id: Message ID to be used
Structured-data: Add structured data to Syslog message. Must be an array of objects with keys “element-id” and “parameter” (a single layer object with string key/values)
```

## Output
```yaml
Output-location: Location to store the output data
```

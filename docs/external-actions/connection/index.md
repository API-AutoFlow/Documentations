---
layout: default
title: Connection
nav_order: 6
parent: External Actions
has_children: true
permalink: /docs/external-actions/connection
---
# Connection


## TCP Actions
You can configure TCP Client or TCP Server in API AutoFlow.


| Category  | Action                       | Purpose                       |  Link  |
|:-----------------|:------------------------------|:---------------------------|:---------------------------|
| Connection | **TCP-Send** |  Sends message through identified TCP Client (Connection)  |  [Open Docs]({% link docs/external-actions/connection/tcp-send.md %})  |
| Server | **TCP-Send** |  Sends message through identified TCP Server Connection  | [Open Docs]({% link docs/external-actions/server/tcp-send.md %})  |
| Server | **TCP-Send-All** |  Sends action message to all connections on the identified TCP Server   | [Open Docs]({% link docs/external-actions/server/tcp-send-all.md %})  |
| Communication | **TCP-Send** |  Creates a TCP connection, sends a message, and then disconnects.  |  [Open Docs]({% link docs/external-actions/communication/tcp-send.md %}) |
| Communication | **TCP-Respond** | Can only be used within a server flow and responds on that server connection  |  [Open Docs]({% link docs/external-actions/communication/tcp-respond.md %}) |
| Communication | **TCP-Send-Receive** | Creates a TCP connection, sends a message, waits for response, then disconnects  |  [Open Docs]({% link docs/external-actions/communication/tcp-receive.md %}) |


{: .fs-6 .fw-300 }

---
layout: default
title: Clients
parent: Servers and Clients
has_children: true
permalink: /docs/servers-and-clients/client
nav_order: 19
---

# Clients
Persistent connections to external services can be created and managed using API AutoFlow.

Currently, supported protocols are

{:toc}

![Create Connection](/assets/images/connections-1.png)

## Creating a new client
Connections can be created by clicking on the [Create New] button. Each type of client requires different sets of information.

![Create Connection](/assets/images/connections-2.png)

Currently, the name has to be unique across the solution configuration to avoid confusion. This may be relaxed in the future.

## Managing clients
Once connection has been created successfully, following connection item is added to the connections list view.
![Connection](/assets/images/connections-3.png)

Click on the newly created connection to go into its configuration view.
![Connection](/assets/images/connections-4.png)

The connection configuration view shows its settings that can be modified as well as the events that it handles. For TCP Client, “connected”, “disconnected”, and “received” events are shown above.

## Configuring clients
You can click on an event to configure its flow. You can also configure the events from the solution page as below.
![Connection](/assets/images/connections-5.png)

## Interacting with the clients
TCP related connection or communication actions can be used to interact with the connection.
![Connection](/assets/images/connections-6.png)

![Connection](/assets/images/connections-7.png)

---
layout: default
title: Data Simulator
parent: Definitions
grand_parent: Overview
has_children: true
permalink: /docs/internal-actions/key-concepts/data-simulator
nav_order: 8
---

# Data Simulator
Mock data is simulated or made-up data for the purpose of testing the solution during development. There are two types of Data Simulation in API AutoFlow.

<details open markdown="block">
  {: .text-delta }
* TOC
{:toc}
</details>


<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips

> **Simulated data ONLY exists within the product**


## Simulating HTTP Request data
The process of creating a flow is to design a chain of actions that provides desired response to the request.  By simulating the request data within the product, developers can visualize the expected response as the flow is built and actions are applied.

## Simulating Actions Response data
Database and communication actions receive data from another server.  During development, it may not be ideal to execute those actions too many times for reasons such as rate limiting and slow responses delaying the development process.

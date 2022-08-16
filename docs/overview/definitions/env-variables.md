---
layout: default
title: Environment (Global) Variable
parent: Definitions
grand_parent: Overview
nav_order: 15
---
# Environment (Global) Variable
A global variable that can be reused throughout the solution.  The environment variable is commonly used to store id, password, IP address, database schema, and more.

## Secret mode
Enables the value to be masked.

![API AutoFlow Environment Variable](/assets/images/env-variable.png)

<img src="/assets/images/tip-icon.png" alt="!" width="20"/>  Tips
> Use Object or Array data type to store multiple values in the environment variable. If only a String data type is used to store a single value, multiple data/get-variable actions need to be used to access the individual value.

## Accessing the data
Use action **[data/get-variable](https://docs.apiautoflow.com/docs/internal-actions/data/get-variable/)** to access the data or from the data-type selection.

Subsequently, you can get the environment variable from the data-type drop-down.

![API AutoFlow Environment Variable Access](/assets/images/env-variable-access.png)

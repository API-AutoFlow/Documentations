---
layout: default
title: Object Data
parent: Oracle ORDS
grand_parent: Databases
---

# Object Data
{: .no_toc }

Gets data from Oracle Database using Oracle Rest Data Services (ORDS).

## Properties

Host: Host address of ORDS endpoint (if scheme is not included, defaults to HTTP)
Port: Port address of ORDS endpoint (could be left empty)
Schema: Schema Alias
Object: Object Alias
Token: OAuth Token obtained using get-auth-token action
Offset: Offset of data to be received usually used for paging
Limit: Limit of data to be received usually used for paging
Filter: Object value with key and values defined according to FilterClause specification

## Output
Output-location: Location to store the output data.

---
layout: default
title: Upsert
parent: Oracle ORDS
grand_parent: Databases
---

# Upsert
{: .no_toc }

Updates a row if key exists, or Inserts a row if key does not exists to Oracle Database using Oracle Rest Data Services (ORDS).

## Properties
Host: Host address of ORDS endpoint (if scheme is not included, defaults to HTTP)
Port: Port address of ORDS endpoint (could be left empty)
Schema: Schema Alias
Object: Object Alias
Keys: List of Keys that uniquely identifies a row listed in the key order
Token: OAuth Token obtained using get-auth-token action
Row: Object value with key and values of the row being inserted

## Output
Output-location: Location to store the output data.

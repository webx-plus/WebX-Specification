---
title: Storage
description: Lua V2 Storage API
parent: V2 API
---
# Lua v2 Storage API

This API allows you store data for future visits, domain scoped.

## Storage Table

Functions:

- get(key) - Get the value from key
- set(key, value, options?) - Set a value to a key
  - options.expires - When the value should be deleted, empty or 'never' for never, 'session' for when the browser closes and a number for seconds
- remove(key) - Remove key
- all() - Returns everything as a table

## Support

{% include support.html table="lua-2/storage" %}

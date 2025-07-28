---
title: Get
description: Lua legacy get
parent: Legacy API
---
# Lua Legacy Get

This global function gets a [element](../element.md) with the name or class passed to it.

{: .deprecated }
This is part of the legacy api which is deprecated and no longer maintained.

```lua
get('links', true)
```

## Inputs

- Name - the name of the tag or class to get
- All - if to get the first or all occurrences

## Return

If `all` set to false: [Element](../element.md)\
If `all` set to true: array of [Element](../element.md)s

## Support

|      | Napture                  | Bussinga                 | YAB                    | WXV Core            |
| ---- | :----------------------: | :----------------------: | :--------------------: | :-----------------: |
| get  | <span full>v1.0.0</span> | <span full>v0.0.1</span> | <span none>None</span> | <span full>1</span> |
| name | <span full>v1.0.0</span> | <span full>v0.0.1</span> | <span none>None</span> | <span full>1</span> |
| all  | <span full>v1.0.0</span> | <span full>v0.0.1</span> | <span none>None</span> | <span full>1</span> |

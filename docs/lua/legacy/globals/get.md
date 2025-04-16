# Lua Legacy Get
This global function gets a [element](../element.md) with the name or class passed to it.

<div style="padding:5px;border:2px #f00 solid;border-radius:5rem;background:#f005;">
  <b>Deprecated:</b> This is part of the legacy api which is deprecated and no longer mantained.
</div>

```lua
get('links', true)
```

## Inputs
- Name - the name of the tag or class to get
- All - if to get the first or all ocurrences

## Return
If `all` set to false: [Element](../element.md)\
If `all` set to true: array of [Element](../element.md)s

## Suport

|      | Napture | Bussinga | YAB  | WXV  |
| ---- | ------- | -------- | ---- | ---- |
| get  | Full    | Full     | Full | Full |
| name | Full    | Full     | Full | Full |
| all  | Full    | Full     | Full | Full |
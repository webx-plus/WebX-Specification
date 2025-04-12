# Lua Legacy Get
This global function gets a element with the name or class passed to it.

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
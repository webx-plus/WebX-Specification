# Lua v2 Browser
This global table holds data about the browser.

```lua
browser.name
```

| Properties | Values |
| Editable   | No     |

## Contents
- name - the name of the browser used
- version - version of the browser used
- api - a table containing info if the browsers support certain apis

### API
The browser should only return the keys with true of the things it supports, everything else should be undefined.\
Contents:
- fetch - the [fetch](fetch.md) api
- get - the [get](get.md) api
- get_type - refers to [getClass](getclass.md), [getId](getid.md) and [getTag](gettag.md)
- print - the [print](print.md) api
- fetch - the [fetch](fetch.md) api

## Suport

|         | YAB  | WXV  |
| ------- | ---- | ---- |
| name    | Full | Full |
| version | Full | Full |
| api     | Full | Full |
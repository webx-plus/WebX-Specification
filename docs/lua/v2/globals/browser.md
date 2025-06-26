---
title: Browser
description: Lua V2 browser table
parent: V2 API
---
# Lua v2 Browser

This global table holds data about the browser.

```lua
browser.name
```

| Properties | Values |
| Editable   | No     |

## Contents

- name - the name of the browser used `Browser name!`
- agent - a normalized version of the name `browser_name`
- version - version of the browser used
- api - a table containing info if the browsers support certain apis

### API

The browser should only return the keys with true of the things it supports, everything else should be undefined.\
Contents:

- fetch - the [fetch](fetch.md) api
- get - the [get](get.md) api
- get_type - refers to [getClass](getclass.md), [getId](getid.md) and [getTag](gettag.md)
- print - refers to [print](print.md), [printe](printe.md) and [printw](printw.md)
- fetch - the [fetch](fetch.md) api

## Support

|         | YAB  | WXV Core |
| ------- | :--: | :------: |
| name    | None | Full     |
| agent   | None | Full     |
| version | None | Full     |
| api     | None | Full     |

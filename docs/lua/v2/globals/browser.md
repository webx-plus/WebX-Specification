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

- name - The name of the browser used `Browser name!`
- agent - A normalized version of the name `browser_name`
- version - Version of the browser used
- api - A table containing info if the browsers support certain apis
- storage - A way to store data, [refer to here](../storage.md)

### API

The browser should only return the keys with true of the things it supports, everything else should be undefined.\
Contents:

- fetch - The [fetch](fetch.md) api
- get - The [get](get.md) api
- get_type - Refers to [get_class](get-class.md), [get_id](get-id.md) and [get_tag](get-tag.md)
- print - Refers to [print](print.md), [printe](printe.md) and [printw](printw.md)
- media_context - The [media_context](../media-context.md) api

## Support

|         | YAB                    | WXV Core            |
| ------- | :--------------------: | :-----------------: |
| name    | <span none>None</span> | <span full>1</span> |
| agent   | <span none>None</span> | <span full>1</span> |
| version | <span none>None</span> | <span full>1</span> |
| api     | <span none>None</span> | <span full>1</span> |
| storage | <span none>None</span> | <span full>2</span> |

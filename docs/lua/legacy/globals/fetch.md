---
title: Fetch
description: Lua legacy fetch
parent: Legacy API
---
# Lua Legacy Fetch

This global function fetches content from the web in a synchronous way.

{: .deprecated }
This is part of the legacy api which is deprecated and no longer maintained.

```lua
local res = fetch({
  url = "https://dns-one.webxplus.org/",
  method = "GET",
  headers = { ["Content-Type"] = "application/json" },
  body = '{ "test": "cat" }'
})
```

## Inputs

- Options
  - URL - if to get the first or all occurrences
  - Method - if to get the first or all occurrences
  - Headers - if to get the first or all occurrences
  - Body - if to get the first or all occurrences

## Return

String or Table (JSON/Object like structure) depending on the response of the fetch.

## Support

|                 | Napture                     | Bussinga                    | YAB                    | WXV Core            |
| --------------- | :-------------------------: | :-------------------------: | :--------------------: | :-----------------: |
| fetch           | <span full>v1.0.0</span>    | <span partial>v0.0.1</span> | <span none>None</span> | <span full>1</span> |
| options.url     | <span full>v1.0.0</span>    | <span none>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| options.method  | <span partial>v1.0.0</span> | <span none>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| options.headers | <span full>v1.0.0</span>    | <span none>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| options.body    | <span full>v1.0.0</span>    | <span none>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |

*fetch some issues around sync present
*options.method Napture only supports GET, POST, PUT, DELETE

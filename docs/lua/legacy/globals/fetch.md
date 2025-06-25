---
title: Fetch
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

|                 | Napture | Bussinga | YAB  | WXV  | WXB  |
| --------------- | :-----: | :------: | :--: | :--: | :--: |
| fetch           | Full    | Full *   | Full | Full | Full |
| options.url     | Full    | Full     | Full | Full | Full |
| options.method  | Full *  | Full     | Full | Full | Full |
| options.headers | Full    | Full     | Full | Full | Full |
| options.body    | Full    | Full     | Full | Full | Full |

*fetch some issues around sync present
*options.method Napture only supports GET, POST, PUT, DELETE

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
  url = "https://dns.webxplus.org/resolve/search/app",
  method = "GET",
  headers = { ["Content-Type"] = "application/json" },
  body = '{ "test": "cat" }'
})
```

## Inputs

- Options
  - URL - The url to fetch
  - Method - Any valid http method (Optional)
  - Headers - Headers to use in the request (Optional)
  - Body - A body in the request (Ignored for GET and HEAD) (Optional)

## Return

String or Table (JSON/Object like structure) depending on the response of the fetch.

## Support

|         | Napture                     | Bussinga                    | WXV Core            |
| ------- | :-------------------------: | :-------------------------: | :-----------------: |
| fetch   | <span full>v1.0.0</span>    | <span partial>v0.0.1</span> | <span full>1</span> |
| url     | <span full>v1.0.0</span>    | <span full>v0.0.1</span>    | <span full>1</span> |
| method  | <span partial>v1.0.0</span> | <span full>v0.0.1</span>    | <span full>1</span> |
| headers | <span full>v1.0.0</span>    | <span full>v0.0.1</span>    | <span full>1</span> |
| body    | <span full>v1.0.0</span>    | <span full>v0.0.1</span>    | <span full>1</span> |

*fetch Bussinga has some issues around async present\
*method Napture only supports GET, POST, PUT, DELETE

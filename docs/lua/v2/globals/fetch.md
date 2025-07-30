---
title: Fetch
description: Lua V2 fetch
parent: V2 API
---
# Lua v2 Fetch

A global function fetches content from the web in a asynchronous way.

```lua
local res = fetch({
  url = "https://dns.webxplus.org/v2/resolve/search/app",
  method = "GET",
  headers = { ["Content-Type"] = "application/json" },
  body = '{ "test": "cat" }'
}):await()
```

{: .note }
Since fetch is async, you need to eventually await it with `:await()` to recive the response

## Inputs

- Options
  - URL - The url to fetch
  - Method - Any valid http method (Optional)
  - Headers - Headers to use in the request (Optional)
  - Body - A body in the request (Ignored for GET and HEAD) (Optional)

## Return

A table with various values about the response.

- status - The response status
- headers - The response headers
- body - The response, Text or a Table depending on the response type.

## Support

|         | YAB                    | WXV Core            |
| ------- | :--------------------: | :-----------------: |
| fetch   | <span none>None</span> | <span full>1</span> |
| url     | <span none>None</span> | <span full>1</span> |
| method  | <span none>None</span> | <span full>1</span> |
| headers | <span none>None</span> | <span full>1</span> |
| body    | <span none>None</span> | <span full>1</span> |

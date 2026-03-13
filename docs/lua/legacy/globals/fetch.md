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

{% include support.html table="lua-legacy/fetch" legacy="true" %}

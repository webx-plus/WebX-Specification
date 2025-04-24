---
title: Window
parent: Legacy API
---
# Lua Legacy Window
This global table holds data about some things.

{: .deprecated }
This is part of the legacy api which is deprecated and no longer mantained.

```lua
window.browser
```

| Properties | Values |
| Editable   | No     |

## Contents
- browser - the name of the browser used
- location - url of the website
- query - query parameters

### Query
The query is a table with key being the param name and value its value. Some important things:
- Last is saved. `?cat=1&cat=2` then `{ cat: '2' }`.
- Case sensative. `?Cat=1&cat=2` then `{ Cat: '1', cat: '2' }`.
- Spaces are not removed. `? cat = 1 ` then `{ ' cat ': ' 1 ' }`.

## Suport

|              | Napture | Bussinga | YAB      | WXV      |
| ------------ | ------- | -------- | -------- | -------- |
| window       | None    | Full     | Full     | Full     |
| browser      | None    | Full     | Full *   | Full *   |
| true_browser | None    | None     | Included | Included |
| location     | None    | Full     | Full     | Full     |
| query        | None    | Full     | Full     | Full     |

*window.browser imitates bussinga's agent, the true client can be accessed in true_browser
# Lua Legacy Window
This global table holds data about some things.

```lua
window.browser
```

## Contents
- browser - the name of the browser used
- location - url of the website
- query - query parameters

## Suport

|          | Napture | Bussinga | YAB    | WXV    |
| -------- | ------- | -------- | ------ | ------ |
| window   | None    | Full     | Full   | Full   |
| browser  | None    | Full     | Full * | Full * |
| location | None    | Full     | Full   | Full   |
| query    | None    | Full     | Full   | Full   |

*window.browser imitates bussinga's agent, the true client can be accessed in true_browser
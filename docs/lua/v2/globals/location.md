---
title: Location
parent: V2 API
---
# Lua v2 Location
This global table holds data about the url/location.

```lua
location.href
```

| Properties | Values |
| Editable   | No     |

## Contents
- href - the complete url `buss://website.it/path?query=params`
- domain - the domain `website.it`
- protocol - protocol `buss`
- path - path `/path`
- query - query parameters `{ query: 'params' }`
- rawQuery - unparsed query parameters `?query=params`
- go(url) - redirect to another url

### Query
The query is a table with key being the param name and value its value. Some important things:
- Duplicate last overwrites others. `?cat=1&cat=2` then `{ cat: '1' }`.
- Case sensitive. `?Cat=1&cat=2` then `{ Cat: '1', cat: '2' }`.
- Multi = are not ignored. `?cat=1=2` then `{ cat: '1=2' }`.
- Spaces are encoded. `?kitty cat=makes meow` then `{ 'kitty%20cat': 'makes%20meow' }`.
- Trailing spaces are trimmed. `? cat = 1 ` then `{ cat: '1' }`.
- Blank values are fine but blank keys are not. `?cat=&=cat&dog&&=` then `{ cat: '', dog: '' }`.
- Trailing ? & are ignored. `?cat&` then `{ cat: '' }` or `?` then `{}`.

## Suport

|          |  YAB  | WXV  |
| -------- |  ---- | ---- |
| location |  Full | Full |
| href     |  Full | Full |
| domain   |  Full | Full |
| protocol |  Full | Full |
| path     |  Full | Full |
| query    |  Full | Full |
| rawQuery |  Full | Full |
| go       |  Full | Full |
| path     |  Full | Full |
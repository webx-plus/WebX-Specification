---
title: Location
description: Lua V2 location table
parent: V2 API
---
# Lua v2 Location

This global table holds data about the URL/location.

```lua
location.href
```

| Properties | Values |
| ---------- | :----: |
| Editable   | No     |

## Contents

- href - the complete URL `buss://website.it/path?query=params`
- domain - the domain `website.it`
- protocol - protocol `buss`
- path - path `/path`
- query - query parameters `{ query: 'params and stuff' }`
- rawQuery - unparsed query parameters `?query=params%20and%20stuff`
- go(url) - redirect to another URL

### Query

The query is a table with key being the param name and value its value. Some important things:

- Duplicate last overwrites others. `?cat=1&cat=2` then `{ cat: '1' }`.
- Case sensitive. `?Cat=1&cat=2` then `{ Cat: '1', cat: '2' }`.
- Multi = are not ignored. `?cat=1=2` then `{ cat: '1=2' }`.
- Special characters are decoded. `?kitty%20cat=makes%20meow` then `{ 'kitty cat': 'makes meow' }`.
- Trailing spaces are trimmed. `?%20cat%20=%201%20` then `{ cat: '1' }`.
- Blank values are fine but blank keys are not. `?cat=&=cat&dog&&=` then `{ cat: '', dog: '' }`.
- Trailing ? & are ignored. `?cat&` then `{ cat: '' }` or `?` then `{}`.

## Support

|          | YAB  | WXV Core |
| -------- | :--: | :------: |
| location | None | Full     |
| href     | None | Full     |
| domain   | None | Full     |
| protocol | None | Full     |
| path     | None | Full     |
| query    | None | Full     |
| rawQuery | None | Full     |
| go       | None | Full     |

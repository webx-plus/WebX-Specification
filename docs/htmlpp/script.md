---
title: Script
description: HTML++ Script
parent: HTML++
---
# Script

A script that will run [lua](../lua/index.md) code.\
Self-closing.

```html
<html>
  <head>
    ...
    <script src="script.lua" version="legacy">
  </head>
  <body>
    ...
    <script src="script.lua" version="2">
  </body>
</html>
```

## Content

None

## Attributes

- Src - the source of the script
- Version - the [lua](../lua/index.md) version to use

### Version

Can be:

- legacy - for the [legacy](../lua/legacy/index.md) api
- 2 - for the [v2](../lua/v2/index.md) api

## Support

|           | Napture                  | Bussinga                 | WXV Core            |
| --------- | :----------------------: | :----------------------: | :-----------------: |
| supported | <span full>v1.0.0</span> | <span full>v0.0.1</span> | <span full>1</span> |
| version   | <span none>None</span>   | <span none>None</span>   | <span full>1</span> |

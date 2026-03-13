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

## Attributes

- src - the source of the script
- version - the [lua](../lua/index.md) version to use

### Version

Can be:

- legacy - for the [legacy](../lua/legacy/index.md) api
- 2 - for the [v2](../lua/v2/index.md) api

## Support

{% include support.html table="htmlpp/script" legacy="true" %}

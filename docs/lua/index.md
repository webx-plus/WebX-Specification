---
title: Lua
description: Lua specification
nav_order: 3
---
# Lua

The programming language of WebX.

## Versions

The Lua API is separated in versions, currently [Legacy](legacy/index.md) and [v2](v2/index.md) are available.\
These can be set like:

```html
<script src="..."> <!-- Defaults to legacy -->
<script api="legacy" src="...">
<script api="v2" src="...">
```

If no version provided will default to legacy.

## Support

| Browser                             | Legacy | v2  |
| ----------------------------------- | :----: | :-: |
| [Napture](../browsers/napture.md)   | Yes    | No  |
| [Bussinga](../browsers/bussinga.md) | Yes    | No  |
| [YAB](../browsers/yab.md)           | Yes    | Yes |
| [WXV](../browsers/wxv.md)           | Yes    | Yes |
| [WebXBrowser](../browsers/wxb.md)   | Yes    | Yes |

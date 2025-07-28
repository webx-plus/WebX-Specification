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

| Browser                             | Legacy                | v2                    |
| ----------------------------------- | :-------------------: | :-------------------: |
| [Napture](../browsers/napture.md)   | <span full>Yes</span> | <span none>No</span>  |
| [Bussinga](../browsers/bussinga.md) | <span full>Yes</span> | <span none>No</span>  |
| [YAB](../browsers/yab.md)           | <span full>Yes</span> | <span full>Yes</span> |
| [WXV](../browsers/wxv.md)           | <span full>Yes</span> | <span full>Yes</span> |
| [WebXBrowser](../browsers/wxb.md)   | <span full>Yes</span> | <span full>Yes</span> |

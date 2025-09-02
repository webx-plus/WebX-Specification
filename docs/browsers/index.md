---
title: Browsers
description: All the browsers that work with WebX.
nav_order: 4
---
# Browsers

All browsers that work with WebX.

- [Napture](napture.md)
- [Bussinga](bussinga.md)
- [YAB](yab.md)
- [WXV](wxv.md)
- [WebXBrowser](wxb.md)

## Browser development

If you want to participate in browser development, refer to the [guide](dev.md).

## Other browser info

| Browser                                      | Language | Viewer Engine | Lua Engine | Platforms                 |
| -------------------------------------------- | -------- | ------------- | ---------- | ------------------------- |
| <img src="napture.png" width="25"> Napture   | Rust     | B9            | Luau       | Windows/Linux             |
| <img src="bussinga.png" width="25"> Bussinga | JS       | Bussinga      | Wasmoon    | Windows/Linux             |
| <img src="yab.png" width="25"> YAB           | JS       | YAB Viewer    | Wasmoon as | Windows/Linux             |
| <img src="wxv.png" width="25"> WXV           | JS       | WXV Core      | Wasmoon as | Web Windows/Linux Android |
| WebXBrowser                                  | C        | WXV Core      | Wasmoon as | Linux                     |

Note: [Wasmoon as](https://www.npmjs.com/package/wasmoon-async-fix) refers to a modified version of wasmoon that includes a fix for async
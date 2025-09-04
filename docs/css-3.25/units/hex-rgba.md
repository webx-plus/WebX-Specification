---
title: Hex RGBA
description: CSS hex rgba unit
parent: Units
---
# Hex RGBA

A [\<color>](../data-types/color.md) type unit that defines rgba color value.

```css
#<number>
#ff00ff
```

## Syntax

`#<number>`

Number must be of length 3, 4, 6 or 8.\
Sizes 3 and 4 need to get each digit doubled, so #845f becomes #884455ff.\
The 4th or 7th and 8th digits represent alpha, if not present it should be the same as fully opaque or FF.

## Support

|           | Napture                  | Bussinga                 | YAB                    | WXV Core            |
| --------- | :----------------------: | :----------------------: | :--------------------: | :-----------------: |
| supported | <span full>v1.0.0</span> | <span full>v0.0.1</span> | <span none>None</span> | <span full>1</span> |

---
title: Element
description: Lua V2 Element Table
parent: V2 API
---
# Lua v2 Element Table

Representation of a element in the lua v2 script

## Contents

Properties:

- content - The text inside a element, value of a [input](../../htmlpp/input.md)/[textarea](../../htmlpp/textarea.md)/[select](../../htmlpp/select.md) or src of a [img](../../htmlpp/img.md)/[audio](../../htmlpp/audio.md)/[video](../../htmlpp/video.md)
- tag - The element's tag
- media_context - Only for audio/video, [more info here](./media-context.md)

Functions:

- remove() - Removes the element

Events:

- on_click => callback() - When the element is clicked
- on_input => callback(value) - When text is written/changed in an input/textarea
- on_keypress => callback(key) - When a key is pressed inside an element
- on_load => callback() - When media element loads
- on_submit => callback(value) - When a form is submitted or enter is pressed on a input

## Support

|               | WXV Core            |
| ------------- | :-----------------: |
| element       | <span full>1</span> |
| content       | <span full>1</span> |
| tag           | <span full>3</span> |
| media_context | <span full>1</span> |
| remove        | <span full>1</span> |
| on_click      | <span full>1</span> |
| on_input      | <span full>1</span> |
| on_keypress   | <span full>1</span> |
| on_load       | <span full>1</span> |
| on_submit     | <span full>1</span> |
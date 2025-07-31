---
title: Element
description: Lua V2 Element Table
parent: V2 API
---
# Lua v2 Element Table

Representation of a element in the lua v2 script

## Contents

Properties:

- content - The text inside a element, value of a input/textarea/select or src of a img/audio/video

Functions:

- remove() - Removes the element

Events:

- on_click => callback() - When the element is clicked
- on_input => callback(value) - When text is written/changed in an input/textarea
- on_keypress => callback(key) - When a key is pressed inside an element
- on_load => callback() - When media element loads
- on_submit => callback(value) - When a form is submitted or enter is pressed on a input

## Support

|             | YAB                    | WXV Core            |
| ----------- | :--------------------: | :-----------------: |
| element     | <span none>None</span> | <span full>1</span> |
| content     | <span none>None</span> | <span full>1</span> |
| remove      | <span none>None</span> | <span full>1</span> |
| on_click    | <span none>None</span> | <span full>1</span> |
| on_input    | <span none>None</span> | <span full>1</span> |
| on_keypress | <span none>None</span> | <span full>1</span> |
| on_load     | <span none>None</span> | <span full>1</span> |
| on_submit   | <span none>None</span> | <span full>1</span> |
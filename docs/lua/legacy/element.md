---
title: Element
description: Lua legacy element table
parent: Legacy API
---

# Lua Legacy Element

A table representing actions that can be done to a [HTML++](../../htmlpp/index.md) element.

{: .deprecated }
This is part of the legacy api which is deprecated and no longer maintained.

## Contents

Functions:

- get_contents() - Get the text contents / value of a element
- set_contents(text) - Set the text contents / value of a element
- get_content() - Alias of get_contents()
- set_content(text) - Alias of set_contents()
- get_href() - Gets the href of a element
- set_href(url) - Sets the href of a element
- get_source() - Gets the src of a element
- set_source(url) - Sets the src of a element
- get_opacity() - Gets the opacity of a element 0 to 1
- set_opacity(opacity) - Sets the opacity of a element 0 to 1
- get_css_name() - Get the class or tag of a element
- set_value(value) - Sets the value of a input

Events:

- on_click => callback() - When the element is clicked
- on_input => callback(value) - When text is written/changed in an input
- on_submit => callback(value) - When a form is submitted or enter is pressed on a input

## Support

|              | Napture                  | Bussinga                    | YAB                    | WXV Core            |
| ------------ | :----------------------: | :-------------------------: | :--------------------: | :-----------------: |
| element      | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| get_contents | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| set_contents | <span full>v1.0.0</span> | <span partial>v0.0.1</span> | <span none>None</span> | <span full>1</span> |
| get_content  | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| set_content  | <span full>v1.0.0</span> | <span partial>v0.0.1</span> | <span none>None</span> | <span full>1</span> |
| get_href     | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| set_href     | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| get_source   | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| set_source   | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| get_opacity  | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| set_opacity  | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| get_css_name | <span none>None</span>   | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| set_value    | <span none>None</span>   | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| on_click     | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| on_input     | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |
| on_submit    | <span full>v1.0.0</span> | <span full>v0.0.1</span>    | <span none>None</span> | <span full>1</span> |

*set_content(s) bussinga will set HTML instead of text (This is [unsafe](https://github.com/inventionpro/Bussinga-attack)), for WXV only if set to bussinga mode
*set_value and get_css_name are only available when WXV Core is set to bussinga mode
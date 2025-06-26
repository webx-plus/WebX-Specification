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

- get_contents() - get the text contents / value of a element
- set_contents(text) - set the text contents / value of a element
- get_content() - alias of get_contents()
- set_content(text) - alias of set_contents()
- get_href() - gets the href of a element
- set_href(url) - sets the href of a element
- get_source() - gets the src of a element
- set_source(url) - sets the src of a element
- get_opacity() - gets the opacity of a element 0 to 1
- set_opacity(opacity) - sets the opacity of a element 0 to 1
- get_css_name() - get the class or tag of a element
- set_value(value) - sets the value of a input

Events:

- on_click => callback() - when the element is clicked
- on_input => callback(value) - when text is written/changed in an input
- on_submit => callback(value) - when a form is submitted

## Support

|              | Napture | Bussinga | YAB  | WXV Core |
| ------------ | :-----: | :------: | :--: | :------: |
| element      | Full    | Full     | None | Full     |
| get_contents | Full    | Full     | None | Full     |
| set_contents | Full    | Full *   | None | Full *   |
| get_content  | Full    | Full     | None | Full     |
| set_content  | Full    | Full *   | None | Full *   |
| get_href     | Full    | Full     | None | Full     |
| set_href     | Full    | Full     | None | Full     |
| get_source   | Full    | Full     | None | Full     |
| set_source   | Full    | Full     | None | Full     |
| get_opacity  | Full    | Full     | None | Full     |
| set_opacity  | Full    | Full     | None | Full     |
| get_css_name | None    | Full     | None | Full *   |
| set_value    | None    | Full     | None | Full *   |
| on_click     | Full    | Full     | None | Full     |
| on_input     | Full    | Full     | None | Full     |
| on_submit    | Full    | Full     | None | Full     |

*set_content(s) bussinga will set HTML instead of text (This is [unsafe](https://github.com/inventionpro/Bussinga-attack)), for WXV only if set to bussinga mode
*set_value and get_css_name are only available when WXV Core is set to bussinga mode
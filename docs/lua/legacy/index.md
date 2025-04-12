# Lua legacy api
The original api version of webx made by Facedev.

<div class="notice deprecated">
  This is deprecated and no longer supported.
</div>

## Globals
- print(text)
- get(selector, all)
- fetch(options)
- window

## Tables
### Element
Methods:
- get_contents()
- set_contents(text)
- get_content()
- set_content(text)
- get_href()
- set_href(url)
- get_source()
- set_source(text)
- get_opacity()
- set_opacity(number)
- get_css_name()
- set_value(text)
Events:
- on_click => callback()
- on_input => callback(value)
- on_submit => callback(value)

## Suport
| Globals | Napture | Bussinga | YAB    |
| ------- | ------- | -------- | ------ |
| print   | Full    | Full     | Full   |
| get     | Full    | Full     | Full   |
| fetch   | Full    | Full *   | Full * |
| window  | None    | Full     | Full * |

*fetch some issues present\
*window YAB imitates bussinga's agent, the true client can be accessed in true_browser

| Element      | Napture | Bussinga | YAB  |
| ------------ | ------- | -------- | ---- |
| get_contents | Full    | Full     | Full |
| set_contents | Full    | Full *   | Full |
| get_content  | None    | Full     | Full |
| set_content  | None    | Full *   | Full |
| get_href     | Full    | Full     | Full |
| set_href     | Full    | Full     | Full |
| get_source   | Full    | Full     | Full |
| set_source   | Full    | Full     | Full |
| get_opacity  | Full    | Full     | Full |
| set_opacity  | Full    | Full     | Full |
| get_css_name | None    | Full     | Full |
| set_value    | None    | Full     | Full |

*set_content(s) bussinga will set html instead of text (This could be unsafe)
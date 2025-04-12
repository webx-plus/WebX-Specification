# Lua legacy api
The original api version of webx made by Facedev.

<div class="notice deprecated">
  This is deprecated and no longer supported.
</div>

## Globals
- get(selector, all)
- fetch(options)
- window

## Tables
### Element
- get_contents()
- get_content()
- set_contents(text)
- set_content(text)

## Suport
| Globals | Napture | Bussinga | YAB    |
| :------ | :-----: | :------: | :----: |
| get     | Full    | Full     | Full   |
| fetch   | Full    | Full *   | Full * |
| window  | None    | Full     | Full * |

*fetch some issues present\
*window Yab imitates bussinga's agent

| Element      | Napture | Bussinga | YAB  |
| :----------- | :-----: | :------: | :--: |
| set_contents | Full    | Full     | Full |
| set_content  | None    | Full     | Full |

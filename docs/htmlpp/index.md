---
title: HTML++
nav_order: 2
---
# HTML++
The version of html that WebX uses.\
This is different from HTML5 and has less features.

## Elements
- [a](a.md)
- [audio](audio.md)
- [body](body.md)
- [button](button.md)
- [div](div.md)
- [h1-6](h1-6.md)
- [head](head.md)
- [hr](hr.md)
- [html](html.md)
- [img](img.md)
- [input](input.md)
- [li](li.md)
- [link](link.md)
- [meta](meta.md)
- [ol](ol.md)
- [option](option.md)
- [p](p.md)
- [script](script.md)
- [select](select.md)
- [textarea](textarea.md)
- [title](title.md)
- [ul](ul.md)

## Example
```html
<html>
  <head>
    <title>My WebX+ Site</title>
    <link href=".../favicon.png">

    <meta name="description" content="My extremly cool site.">
    <meta name="theme-color" content="#000000">

    <link href="styles.css">
    <script src="script.lua">
  </head>
  <body>
    <h1>My site</h1>
    <p>Im very cool</p>
  </body>
</html>
```
Unlike HTML5, HTML++:
- doesn't have a `<!DOCTYPE html>`
- doesn't have a rel attribute for [link](link.md), the first link will be the favicon unless its a [css](../css-3.25/index.md) file, the rest will just be trated as [css](../css-3.25/index.md).
- [scripts](script.md) are self-closing, are written in [lua](../lua/index.md) and they can only point to code on another file.

Other:
- the [meta](meta.md) elements provide info for search engines
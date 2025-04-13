# HTML++
The version of html that WebX uses.\
This is different from HTML5 and has less features.

## Elements
- [html](html.md)
- [head](head.md)
- [title](title.md)
- [link](link.md)
- [meta](meta.md)
- [body](body.md)
- [h1-6](h1-6.md)
- [p](p.md)
- [hr](hr.md)
- [div](div.md)
- [input](input.md)
- [textarea](textarea.md)
- [select](select.md)
- [option](option.md)
- [ul](ul.md)
- [ol](ol.md)
- [li](li.md)
- [img](img.md)
- [script](script.md)

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
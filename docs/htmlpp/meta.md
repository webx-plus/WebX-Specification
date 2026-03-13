---
title: Meta
description: HTML++ Meta
parent: HTML++
---
# Meta

Metadata about the site that shows in search engines.\
Self-closing.

```html
<html>
  <head>
    ...
    <meta name="description" content="My cool web">
    <meta name="theme-color" content="#000000">
  </head>
  ...
</html>
```

## Attributes

- name - the name of the metadata to target
- content - the content to assign it

### Name

Currently the following names are supported/used:

- description - a description of the site
- theme-color - a color to show for embeds

Other names can be used but will be ignored by most programs/browsers.

## Support

{% include support.html table="htmlpp/meta" legacy="true" %}

# markdown

The `markdown` module provides helpers for turning markdown into DOM nodes for rendering in the browser.

It's a convenience reference to the [beldown](https://npmjs.com/beldown) module.

## Example usage

```js
var md = require('adventuretron/markdown')

var html = md`
  # hi
 
  this is markdown
`
 
console.log(html.toString())
```

this returns:

```html
<div>
<h1 id="hi">hi</h1>
<p>this is markdown</p>
</div>
```

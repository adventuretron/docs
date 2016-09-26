# html

The `html` module is a convenience reference to [yo-yo](http://npmjs.com/yo-yo), so you can use it exactly the same way as defined in the yo-yo docs.

## Example usage

```js
var html = require('adventuretron/html')

var tree = html`
  <p>this is some html</p>
`

console.log(tree.toString())
// > <p>this is some html</p>
```

The primary use of the `html` module in Adventuretron is creating the DOM nodes that are returned from each challenge's `content` function.

Here's how usage looks in an Adventuretron challenge:

```js
var html = require('adventuretron/html')

var i18n = require('./i18n')

module.exports = {
  i18n: i18n,
  content: function (params, send) {
    var lang = params.language
    var challenge = params.challenge

    return html`<div>
      <p>the content of the challenge</p>
    </div>`
  }
}
```

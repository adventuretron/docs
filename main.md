# main

The `main` module is responsible creating the main window using electron.

## Usage example

For most workshops, you'll create a `main.js` file that looks like this:

```js
var path = require('path')
var adventuretron = require('adventuretron/main')

var app = adventuretron({
  title: 'Example adventuretron workshop',
  index: 'file://' + path.join(__dirname, 'index.html')
})
```

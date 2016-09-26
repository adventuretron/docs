# renderer

The `renderer` module is responsible for all the UI code, the app with all the challenges that users work through.

## Example usage

```js
var path = require('path')
var createApp = require('adventuretron/renderer')
var css = require('sheetify')

css('adventuretron')

var app = createApp({
  name: 'adventuretron-adventure',
  defaultLanguage: 'en',
  languages: {
    'en': 'English',
    'es': 'Español'
  },
  i18n: path.join(__dirname, 'i18n'),
  challenges: path.join(__dirname, 'challenges')
})

app.start()
```

In this example we're using [sheetify](https://npmjs.com/sheetify) to include the basic adventuretron css styles. You can include the css using other methods, but sheetify is recommended.


# description

This helper module returns the content from the description file that matches the current language of the user.

## Usage example

`description` takes two arguments:

- `challenge` – the current challenge
- `lang` - current language of the user

Here's how usage looks inside an Adventuretron challenge:

```js
var html = require('adventuretron/html')
var description = require('adventuretron/description')

var i18n = require('./i18n')

module.exports = {
  i18n: i18n,
  content: function (params, send) {
    var lang = params.language
    var challenge = params.challenge

    return html`<div>
      ${description(challenge, lang)}
    </div>`
  }
}
```
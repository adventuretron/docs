# verify directory

Use this UI component to verify that a user has structured a directory and its files correctly.

## Usage example

```js
var verifyDir = require('adventuretron/verify-directory')

var options = {
  headerText: 'Create some files',
  descriptionText: 'Put files `hi.txt` and `ok.md` in a directory',
  buttonText: 'Check your directory',
  files: ['hi.txt', 'ok.md']
  verify: verify
}

function verify (err, ok) {
  if (err && !ok) {
    // show the error message
  } else {
    // show the success message
  }
}

verifyDir(options)
```

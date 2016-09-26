# verify text

Use this UI component to verify content that a user has placed in a file.

## Usage example

```js
var verifyText = require('adventuretron/verify-text')
var expectedAnswer = 'cool'

var options = {
  headerText: 'Write a function',
  descriptionText: 'The function must return the string "this is fun".',
  buttonText: 'Check your file',
  verify: verify
}

function verify (answer) {
  if (answer && answer === expectedAnswer) {
    // show the success message
  } else {
    // show the error message
  }
}

verifyText(options)
```

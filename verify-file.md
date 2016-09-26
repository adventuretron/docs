# verify file

Use this UI component to verify content that a user has placed in a file.

## Usage example

```js
var verifyFile = require('adventuretron/verify-file')
var expectedAnswer = 'cool'

var options = {
  headerText: 'Write a function',
  descriptionText: 'The function must return the string "this is fun".',
  buttonText: 'Check your file',
  verify: verify
}

function verify (answer) {
  try {
    var answerFunction = new Function('return ' + code)()
    var answer = answerFunction()
  } catch (err) {
    // show the error message
  }

  if (answer && answer === expectedAnswer) {
    // show the success message
  } else {
    // show the error message
  }
}

verifyFile(options)
```

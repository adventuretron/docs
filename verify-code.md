# verify code

Use this UI component to verify code entered by the user.

## Usage example

```js
var verifyCode = require('adventuretron/verify-code')
var expectedAnswer = 'cool'

var options = {
  headerText: 'Write a function',
  descriptionText: 'The function must return the string "this is fun".',
  buttonText: 'Check your code',
  value: value,
  editor: { hideOutput: true },
  verify: verify
}

function verify (code) {
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

verifyCode(options)
```

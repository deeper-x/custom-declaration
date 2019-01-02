# Typescript - Declaration file for a custom module
With this simple example, we show how to define and set up a type definition for a custom Javascript library, in a Typescript module.

We write and publish on npm a test module, a "reverse with sharps" library: given an input string, it returns the reversed version with some sharps around.

Example:
```javascript
console.log(reverseWithSharps("ALBERTO"));

// result: ## OTREBLA ##
```

Then we use it in a TS file, simply defining a declaration file, requiring an input string as a parameter, returning a string as a result:
```javascript
/// <reference path="./reverse-with-sharps.d.ts"/>
import * as myModule from 'reverse-with-sharps';

console.log(myModule.reverseWithSharps("ALBERTO"));

// result: ## OTREBLA ##
```

# Typescript - Declaration file for a custom module
With this simple example, we show how to define and set a type definition for a custom js library, in a Typescript module.

First, we write and publish on npm a "reverse with sharps" module: given an input string, it returns the reversed version with some sharps around.

Example:
```javascript
console.log(reverseWithSharps("ALBERTO"));

// result: ## OTREBLA ##
```

Then, after published on npm, we use it in a ts file, simply defining a .d.ts which require an input string, returning a string:
```javascript
/// <reference path="./reverse-with-sharps.d.ts"/>
import * as myModule from 'reverse-with-sharps';

console.log(myModule.reverseWithSharps("ALBERTO"));

// result: ## OTREBLA ##
```

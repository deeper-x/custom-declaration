# custom-declaration
With this simple example, we show how to include a declaration file for a custom module.
First, we write and publish on npm a "reverse with sharps" module: given an input string, it returns the reversed version with some sharps around.
Example

```javascript
console.log(reverseWithSharps("ALBERTO"));

// result ## OTREBLA ##

```

Then, after published on npm we use it, simply defining a d.ts which require an input string, returning a string.

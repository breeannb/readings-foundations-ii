# Read 01: JS Templates and Array .forEach method

## JS Templates
### [MDN (only read up to (but not including) "Nesting Templates")](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)
> * Template literals are string literals allowing embedded expressions. You can use multi-line strings and string interpolation features with them.
> * Template literals are enclosed by the backtick ` (grave accent) character instead of double or single quotes.
> * To escape a backtick in a template literal, put a backslash (\) before the backtick.
```
`\`` === '`' // --> true
```
> * Multi-line strings - 
Any newline characters inserted in the source are part of the template literal.
> * Expression interpolation - 
``` 
let a = 5;
let b = 10;
console.log('Fifteen is ' + (a + b) + ' and\nnot ' + (2 * a + b) + '.');
// "Fifteen is 15 and
// not 20."
```

### [Google Developer (don't need to read "Tagged Templates")](https://developers.google.com/web/updates/2015/01/ES6-Template-Strings)

> * Template Strings use back-ticks (``) rather than the single or double quotes we're used to with regular strings. A template string could thus be written as follows:

var greeting = `Yo World!`;

> * String Substitution
>   * Substitution allows us to take any valid JavaScript expression (including say, the addition of variables) and inside a Template Literal, the result will be output as part of the same string.
>   * As all string substitutions in Template Strings are JavaScript expressions, we can substitute a lot more than variable names.

> * Multiline Strings
>   * Multiline strings in JavaScript have required hacky workarounds for some time. Current solutions for them require that strings either exist on a single line or be split into multiline strings using a \ (backslash) before each newline.

### [CSS Tricks (don't need to read "Tagged Templates" or following section)](https://css-tricks.com/template-literals/)
> * To create a template literal, instead of single quotes (') or double quotes (") quotes we use the backtick (`) character. This will produce a new string, and we can use it in any way we want. Basic usage:

let newString = `A string`;
> * Multi-line
> * The great thing about Template Literals is that we can now create multi-line strings! In the past, if we wanted a string to be on multiple lines, we had to use the \n or new line character.
```
// The old way
var myMultiString = 'Some text that I want\nOn two lines!';
``` 
>   * With a Template Literal string, we can just go ahead and add the new line into the string as we write it.
```
var myMultiString= `This will be
on two lines!`;
```
> * Expressions
>   * The ${} syntax allows us to put an expression in it and it will produce the value, which in our case above is just a variable that holds a string! There is something to note here: if you wanted to add in values, like above, you do not need to use a Template Literal for the name variable. It could just be a regular string.
> * We can also use this with a more complex object.
```
let person = {
    firstName: `Ryan`,
    lastName: `Christiani`,
    sayName() {
        return `Hi my name is ${this.firstName} ${this.lastName}`;
    }
};
``` 
> * Here we have a person object with a sayName() method on it. We can access the properties from an object inside of the ${} syntax.
> * HTML Templates - With the ability to have multi-line strings and use Template Expressions to add content into our string, this makes it really nice to use for HTML templates in our code.
> * Reusable Templates



## Array Methods

### [MDN forEach](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/forEach)
> * forEach() calls a provided callback function once for each element in an array in ascending order. It is not invoked for index properties that have been deleted or are uninitialized.
> * callback is invoked with three arguments:
>   * the value of the element
>   * the index of the element
>   * the Array object being traversed

### [for vs forEach (No need to read past first two paragraphs of "When to use..." section)](https://medium.com/@abustamam/for-loops-vs-foreach-in-javascript-7a977278a39e)
> * The for loop: learning to count again
> * forEach
>   * forEach is a method on the Array prototype. In other words, you can call it on any array, like so:
> * Callback accepts three arguments: 
>   * element value
>   * element index
>   * array being traversed (I have never used this)
> * When to use a for loop over forEach
> * forEach comes with a little caveat. It only works on arrays. So if you want to actually count, forEach probably isn’t your friend.
# SNOW-ECMAScript-6
ServiceNow is not at this version yet.

```
ECMAScript 6 is also known as ES6 and ECMAScript 2015

JavaScript let
The let statement allows you to declare a variable with block scope.
Example
var x = 10;// Here x is 10{     let x = 2;    // Here x is 2}// Here x is 10
![image](https://user-images.githubusercontent.com/12488769/148699331-ed030cfb-821c-4d22-ad60-8c1cb299689e.png)

```
var is function scoped and let is block scoped.It can be said that a variable declared with var is defined throughout the program as compared to let.

## const
The const statement allows you to declare a constant (a JavaScript variable with a constant value).
Constants are similar to let variables, except that the value cannot be changed.
```
Example
var x = 10;// Here x is 10{     const x = 2;    // Here x is 2}// Here x is 10

```
## default parameter values
ES6 allows function parameters to have default values.
```
Example
function myFunction(x, y = 10) {    // y is 10 if not passed or undefined    return x + y;}myFunction(5); // will return 15
```
## Arrow functions
```
Arrow functions allows a short syntax for writing function expressions.
You don't need the function keyword, the return keyword, and the curly brackets.
Example
// ES5 
var x = function(x, y) 
{return x * y;}
// ES6
var  x = (x, y) => x * y;
```
## The Rest parameter / operator
This operator is an improvement to the way function parameters are handled, allowing us to more easily handle a variable number of function parameters.
```
Snippet :
// es6 rest parameter 
function fun(...input){ 
	let sum = 0; 
	for(let i of input){ 
		sum+=i; 
	} 
	return sum; 
} 
console.log(fun(1,2)); //3 
console.log(fun(1,2,3)); //6 
console.log(fun(1,2,3,4,5)); //15
```
JavaScript Array reduce() Method



## The Spread Operator
When … occurs in function call or alike,its called a spread operator. 

```
The spread operator can be used to turn an array of values onto a set of function parameters. Returning to our add() example:

  function add(...numbersToAdd) { // This is a Rest parameter
  return numbersToAdd.reduce((sum, next) => sum + next);
   }
 
   var numbers = [1, 2, 3];
   add(...numbers); // this is a Spread operator
   // The above is functionally the same as:
   add(1, 2, 3);
```
### Template literals
- Template Literal in ES6 provides new features to create a string that gives more control over dynamic strings. Traditionally, String is created using single quotes (‘) or double quotes (“) quotes. Template literal is created using the backtick (`) character.
- Multiline Strings: In-order to create a multiline string an escape sequence \n was used to give new line character. However, Template Literals there is no need to add \n string ends only when it gets backtick (`) character.






## Data types

### Numbers
The _number_ type represents both integer and floating point numbers.
Besides regular numbers, there are so-called “special numeric values” which also belong to this data type: `Infinity`, `-Infinity` and `NaN`.
 
### Strings
A string in JavaScript must be surrounded by quotes.
```javascript
let str = "Hello";
let str2 = 'Single quotes are ok too';
let phrase = `can embed ${str}`;
```

### Boolean
The boolean type has only two values:  `true`  and  `false`.

This type is commonly used to store yes/no values:  `true`  means “yes, correct”, and  `false`  means “no, incorrect”.

```javascript
let nameFieldChecked = true; // yes, name field is checked
let ageFieldChecked = false; // no, age field is not checked
```
### Object
Objects are used to store collections of data and more complex entities.
```javascript
let user = {     // an object
  name: "John",  // by key "name" store value "John"
  age: 30        // by key "age" store value 30
};
```

### The “null” value
It’s just a special value which represents “nothing”, “empty” or “value unknown”.
```javascript
let age = null;
```

###  Undefined
The meaning of  `undefined`  is “value is not assigned”.

If a variable is declared, but not assigned, then its value is  `undefined`:

```javascript
let x;
alert(x); // shows "undefined"
```

## Variable declaration
A variable declaration introduces a new identifier.
```javascript
  var declaration
  let.log(declaration)  // undefined
  declaration =  'This is an initialization'
  ```
Above we create a new identifier called declaration. In JavaScript, variables are initialized with the value of `undefined` when they are created. What that means is if we try to log the `declaration` variable, we’ll get `undefined`.
In contract to variable declaration, variable initialization is when you first assign a value to a variable.

### Let
The main difference between `var` and `let` is that instead of being function scoped, `let` is block scoped. What that means is that a variable created with the `let` keyword is available inside the “block” that it was created in as well as any nested blocks   like in a `for` loop or an `if` statement.

> var: function scoped 
let: block scoped

### Const
Is a block spcoed  declaration that once you’ve assigned a value to a variable using `const`, you can’t reassign it to a new value.
```javascript
let animal =  'Dog'  
const vehicle =  'car' 
animal =  'cat'  // ✅ 
handle =  'bus'  // ❌ 
```

### Classes
In JavaScript, a class is a kind of a function. Just like functions, classes can be defined inside another expression, passed around, returned, assigned etc.
```javascript
let User = class {
  sayHi() {
    alert("Hello");
  }
};
```
The  `constructor()`  method is called automatically by  `new`, so we can initialize the object there.

For example:

```javascript
class User {
  constructor(name) {
    this.name = name;
  }
  sayHi() {
    alert(this.name);
  }
}
// Usage:
let user = new User("John");
user.sayHi();
```

Class declaration is not hoisted  like a function declaration
```javascript
const user = new User(); //error
class user{}
```


###  Promises & async/await

### Object Destructuring and Spread Syntax

A function can be called with any number of arguments, no matter how it is defined.
```javascript
function sum(a, b) {
  return a + b;
}

alert( sum(1, 2, 3, 4, 5) );
```
There will be no error because of “excessive” arguments. But of course in the result only the first two will be counted.

The rest parameters can be mentioned in a function definition with three dots `...`. They literally mean “gather the remaining parameters into an array”.

```javascript
function showName(firstName, lastName, ...names) {
  alert( firstName + ' ' + lastName ); // Julius Caesar
  alert( names[0] ); // Bart
  alert( names[1] ); // Lisa
  alert( names.length ); // 2
}
showName("Homer", "Marge", "Bart", "Lisa");
```
### Spread operator
Passing an array to parameters
```javascript
let arr = [3, 5, 1];

alert( Math.max(...arr) ); // 5 (spread turns array into a list of arguments)
```
### Arrow Functions
### Generators
### JavaScript Modules
### Declarative vs Imperative (Ver con Tony)
### React intro
### Components
### JSX

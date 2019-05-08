

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
  ```
Above we create a new identifier called declaration. In JavaScript, variables are initialized with the value of `undefined` when they are created. What that means is if we try to log the `declaration` variable, we’ll get `undefined`.

"Classes"
Promises & async/await
Object Destructuring and Spread Syntax
Arrow Functions
Generators
JavaScript Modules
Declarative vs Imperative (Ver con Tony)
React intro
Components
JSX

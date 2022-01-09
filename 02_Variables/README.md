# JavaScript Variables

## 1 - JavaScript Data Types

| Data Types    | Description                                         | Example                          | 
| ------------- | -------------------------------------------         | -------------------------------- |  
| `String`      | 	represents textual data                           | `hello` etc.                     |
| `Number`      | 	an integer or a floating-point number             | `3`, `3.234`, `3e-2`             |
| `BigInt`      | 	an integer with arbitrary precision               | `900719925124740999n`, `1n` etc. |
| `Boolean`     | 	Any of two values: true or false	              | `true` and `false`               |
| `undefined`   | 	a data type whose variable is not initialized     | `let a`;                         |
| `null`        |   denotes a `null` value                            | `let a = null` ;                 |
| `Symbol`      |   data type whose instances are unique and immutable| `let value = Symbol('hello');`   |
| `Object`      |   key-value pairs of collection of data             | `let student = { };`             |


### 1.1 - Primitive Types
- #### String
```javascript
let firstName = 'Çınar';
```
- #### Number
```javascript
let Age = 23;
let money = 100.5; 
```
- #### Boolean
```javascript
let isActive = false;
```

- #### null
```javascript
let job = null;
```
- #### undefined
```javascript
let car;
```
- #### Example
```javascript
let info = "Lorem, ipsum dolor.";
info = 'Lorem, "ipsum" dolor.';
info = `Lorem, "ipsum" dolor.`;

info = "Lorem, \"ipsum\" dolor.";
info = 'Lorem, \'ipsum\' dolor.';
info = `Lorem, \`ipsum\` dolor.`;

info = `Lorem, ${ipsumA} and ${ipsumB}`;
```

### 1.2 - Reference Types
- #### Array
```javascript
let names = ["Ömer", "Faruk", "Mehmet"];

console.log(typeof names); // object 
```

- #### Object
```javascript
let address = {
    city : 'İstanbul',
    country : 'Turkey'
}
console.log(typeof address); // object 
```
- ### Function
```javascript
var calculateAge = function(){
    return 0;
}
console.log(typeof calculateAge); // function 
```

### Naming JavaScript Variables

```javascript
let 1test;  // error
let for;    // error
var switch; // error

let test1;
let _test2;
let $test3;
```

##### Case Sensitive 

```javascript
var firstName = "Faruk OKUTAN";

var firstname = "Faruk OKUTAN";

var first_name = "Faruk OKUTAN";
```

## 2 - Variable Keyword (Var, Let, Const)

### 2.1 - Var Example 
var variables can be re-declared and updated

```javascript
var year = 2021;

var year = 2022;

year = 2023;

(this will return an error)
let year   = 2019; // SyntaxError: Identifier 'year' has already been declared
const year = 2025; // SyntaxError: Identifier 'year' has already been declared
```

### 2.2 - Let Example
let can be updated but not re-declared.

```javascript
let message = "Hi, Faruk";

message = "Hello, Faruk";

(this will return an error)
let message = "Hello, Mr. Faruk"; // SyntaxError: Identifier 'message' has already been declared
```

### 2.3 - Const Example
const declarations are `block` scoped

```javascript
const nationalID = "A12B3C45DEF6";

(this will return an error)
nationalID = "ABCDEF987654";       // TypeError: Assignment to constant variable.
const nationalID = "ABCDEF987654"; // SyntaxError: Identifier 'message' has already been declared
let nationalID   = "ABCDEF987654"; // SyntaxError: Identifier 'message' has already been declared
```

---
> "JavaScript Data Types", [Link](https://www.programiz.com/javascript/data-types)
---
> "Var, Let, and Const – What's the Difference?", [Link](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/)
---
> "JavaScript Primitive vs Reference types", [Link](https://dev.to/ykhokhaneshiya/javascript-primitive-vs-reference-types-43dl)
---
> Softtech Course Study Notes

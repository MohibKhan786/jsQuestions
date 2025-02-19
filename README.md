# Questions on [let var const] By Hussain Sarfaraz

## Basic Multiple-Choice Questions:

1. In JavaScript, what is the scope of a variable declared with var?

    a) Global scope
  
    b) Function scope
  
    c) Block scope
  
    d) Module scope
  

2. What happens if you declare a variable with var inside a block statement (e.g., if, for, while)?

    a) The variable has block scope.
    
    
    b) The variable has function scope.
    
    
    c) The variable has global scope.
    
    
    d) The variable is not affected by the block statement.



3. What is the behavior of hoisting for variables declared with var?

    a) Variables are hoisted and can be accessed anywhere within the function or global scope.
    
    
    b) Variables are hoisted only within the block where they are declared.
    
    
    c) Variables are not hoisted, and referencing them before declaration results in an error.
    
    
    d) Variables are hoisted, but they retain their value at the time of declaration.



4. In a function, if a variable is declared with var inside the function and is not explicitly returned, what is the scope of that variable?

    a) Global scope
    
    
    b) Function scope
    
    
    c) Module scope
    
    
    d) Block scope



5. When using var to declare a variable with the same name inside a function and in the global scope, what happens?

    a) The variable inside the function shadows the global variable.
    
    b) An error is thrown because the variable name is already used in the global scope.
    
    c) Both variables coexist, and the function will use the local variable first.
    
    d) The global variable gets reassigned with the value of the local variable.


6. In JavaScript, what is the behavior of re-declaring a variable with var within the same scope?

    a) The variable is re-initialized to its original value.
    
    b) A new variable is created with the same name, shadowing the original variable.
    
    c) An error is thrown because you cannot re-declare a variable with var.
    
    d) The new declaration has no effect; it continues to reference the original variable.

7. What happens if a variable is declared inside a function and also declared with var in the global scope?

    a) Both variables are accessible globally but hold different values.
    
    b) An error is thrown because you cannot have the same variable name declared multiple times.
    
    c) The global declaration is ignored, and the variable inside the function is used.
    
    d) The global declaration overrides the local declaration inside the function.

8. What is the value of y after the following code is executed?
  ```js
  var x = 5;
  function foo() {
    var x = 10;
  }
  foo();
  var y = x;
  ```
    a) 5
    
    b) 10
    
    c) undefined
    
    d) ReferenceError

9. What is the output of the following code?
  ```js# JS-Questions
  console.log(x);
  var x = 10;
  
  ```
    a) ReferenceError: x is not defined
    
    b) undefined
    
    c) null
    
    d) 10

10. What will the code output?
  ```js
  var x = 5;
  if (true) {
    var x = 10;
  }
  console.log(x);
  
  ```
    a) 5
    b) 10
    c) undefined
    d) ReferenceError


## Predict the output type questions?

  1. 
    ```js  const pi=3.14
      console.log(pi)
      pi=3;
    function foo() {
      console.log(x);
      var x = 5;
    }
    foo();
    
    ```
  
  2. 
    ```js
    
    for (var i = 0; i < 3; i++) {
      setTimeout(function () {
        console.log(i);
      }, 100);
    }
    
    ```

  3.
    ```js
    var x = 10;
    if (true) {
      var x = 20;
    }
    console.log(x);
    ```

  4.
    ```js
    
    var x = 5;
    function foo() {
      console.log(x);
      var x = 10;
    }
    foo();
    
    ```

  5.
    ```js
    var x = 5;
    function foo() {
      console.log(x);
    }
    foo();
    
    ```
  
  6.
    ```js
    
    var x = 1;
    if (true) {
      var x = 2;
      console.log(x);
    }
    console.log(x);
  
    ```

  7.
    ```js
    
    var x = 10;
    function foo() {
      console.log(x);
    }
    foo();
    
    ```

  8.
    ```js
    var x = 5;
    if (true) {
      var x = 10;
      console.log(x);
    }
    console.log(x);
    
    ```
  
  9.
    ```js
    for (var i = 0; i < 5; i++) {
      setTimeout(function () {
        console.log(i);
      }, 100);
    }
    
    ```
  
  10. 
    ```js# JS-Questions
    function foo() {
      var x = 5;
    }
    foo();
    console.log(x);
    
    ```


## ADVANCE Theory questions

1. What is the temporal dead zone in relation to let?

2. How does let differ from var in terms of hoisting and scope?

3. Explain how let variables are affected by closures in JavaScript.

4. Compare and contrast the behavior of let and const when used in loops and conditional statements.

5. What are the best practices for using let in modern JavaScript development?

6. How does the usage of let impact garbage collection and memory management in JavaScript?

7. Describe the lexical scoping rules that apply to let variables in arrow functions.

8. Explain the behavior of let when used inside async functions and how it handles asyn# Node.js template



# * * * Md Mohib Khan * * *

## Group-A (Write output:)

### 1) 
  ```
  const pi=3.14
  console.log(pi)
  pi=3;

  ```
### 2) 
  ```
  function foo(){
    var n=6;
    console.log(n);
  }
  var n=5;
  console.log(n);
  foo();

  ```
### 3)
```
 function foo(n) {
    if (n == 6) {
        let num = 2;
    }
    console.log(num);
 }

 var n = 6;
 console.log(n);
 foo(6);
```

### 4)
```
function foo(n) {
    if (n === 6) {
        var num = 2;
    }
    console.log(num);
}
var n = 6;
console.log(n);
foo(n);

```
### 5)
```
for(var i=0;i<3;i++){
  console.log(i)
 }
 console.log("i outside the loop: ", i);

 for(let j=0;j<3;j++){
  console.log(j);
 }
 console.log("j oustide the loop :", j);
```

### 6)
```
x = 2
var y = x + 1
console.log(y)
var x;
```

### 7)
```
var y = x + 1
console.log(x) 
console.log(y) 
var x = 2;
```
### 8)
```
for (let i = 0; i < 5; i++) {
  setTimeout(() => console.log(i))
}
```

### 9)
```
let { g, ...h } = { a: 1, g: 2 }
console.log(g, h) 
```

### 10)
```
const fruit = 'apple'
{
  const fruit = 'orange'
  console.log(fruit) 
}
console.log(fruit) 
```
    
## Group-B

### 11) Which of the following is true about const?

     a) It creates a read-only reference to a value.
    
     b) It creates an immutable object.
     
     c) It can't be used in strict mode.
     
     d) It allows reassignment just like let.

### 12) When should you use const over let? 

     a) When the variable needs to be reassigned.
     
     b) When the variable's value will never change.
     
     c) When you want to prevent variable hoisting.
     
     d) When you want to avoid using block scope.

### 13) What is the value of a variable declared with const that is not initialised during declaration? 

    A) null 
    
    B) undefined
    
    C) 0
    
    D) It throws a syntax error.

### 14) Which type of variable declaration is recommended when you need to reassign the variable later? 

    A) const 
    
    B) let
    
    C) var 
    
    D) All of them are equally suitable.

### 15) Which of the following declarations is not valid in strict mode? 

    A) var x = 10; 
    
    B) let x = 10;
    
    C) const x = 10; 
    
    D) All of them are valid.
                






    

# Aasif Iqbal
## (Guess the output)
01. var 
```
var fruit = 'apple'
{
  var fruit = 'orange'
  console.log(fruit) // ??
}

console.log(fruit) // ??
```
02. var
```
var fruit = 'apple'

function gimmeFruit() {
  var fruit = 'orange'
  console.log(fruit) // ??
}

console.log(fruit) // ??
gimmeFruit()
```
03. let
```
let fruit = 'apple'

{
  let fruit = 'orange'
  console.log(fruit) // ??
}

console.log(fruit) // ??
```
04. let
```
function foo(n) {
    if (n == 6) {
        let num = 2;
    }
    console.log(num);
}

var n = 6;
console.log(n);
foo(6);
```
05. let
```
for(var i=0;i<3;i++){
  console.log(i)
}
console.log("i outside the loop: ", i);

for(let j=0;j<3;j++){
  console.log(j);
}

console.log("j oustide the loop :", j);
```
06. const
```
{
  const fruit = 'apple'
  fruit = 'orange'
  console.log(fruit)
}
```
07. const
```
if (true) const a = 1;
```
08. const
```
const MY_FAV = 7;

if (MY_FAV === 7) {
   
  const MY_FAV = 20;
  console.log(MY_FAV);  
  
  var MY_FAV = 20;  
}

console.log(MY_FAV); 
```
09. let and var
```
{  
  console.log(bar);  
  console.log(foo);  
  var bar = 1;
  let foo = 2;  
}
hint:TDZ
```
10. let and var
```
{

  const func = () => console.log(letVar);

  let letVar = 3; 
  func(); 
}

```
11. let and var
```
function test() {
  var foo = 33;
  if (foo) {
    let foo = foo + 55; 
  }
}
test();

```
12. let and var
```
function go(n) {
  
  console.log(n); 

  for (let n of n.a) {
  
    console.log(n);
  }
}

go({ a: [1, 2, 3] });

```
13. let and var
```
let x = 1;

{
  var x = 2; 
}

```
14. var
```
"use strict";
var x = 1;
Object.hasOwn(globalThis, "x"); // ??
delete globalThis.x; // ??
delete x; // ??

```
15. var
```
try {
  throw 1;
} catch (e) {
  var e = 2; 
}
console.log(e); // ??

```
16. var
```
"use strict";

var x = 0;
function f() {
  var x = y = 1;
}
f();

console.log(x, y);

```
17. var
```
function foo(a) {
  var a = 1;
  console.log(a);
}

foo(2); 
 ```     





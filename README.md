# jsQuestions

# Node.js template

This is a Node.js project.

Add your [configuration](https://codesandbox.io/docs/projects/learn/setting-up/tasks) to optimize it for [CodeSandbox](https://codesandbox.io/p/dashboard).

## Resources

- [CodeSandbox — Docs](https://codesandbox.io/docs/projects)
- [CodeSandbox — Discord](https://discord.gg/Ggarp3pX5H)



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
```js
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
```js
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
```js
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

Compare and contrast the behavior of let and const when used in loops and conditional statements.

What are the best practices for using let in modern JavaScript development?

How does the usage of let impact garbage collection and memory management in JavaScript?

Describe the lexical scoping rules that apply to let variables in arrow functions.

Explain the behavior of let when used inside async functions and how it handles asynchronous operations.

Discuss the implications of using let in multi-threaded environments, such as web workers or Node.js clusters.

Write a detailed comparison of let and var in terms of their performance, readability, and potential pitfalls.


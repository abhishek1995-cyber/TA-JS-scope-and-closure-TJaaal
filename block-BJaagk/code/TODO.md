1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Your code goes here
let percentage = function percentage(marks,total) {
  return (marks * 100) / total;
}
let percentage = function (marks,total) {
  return (marks * 100) / total;
}
let percentage = (marks,total) => {
  return (marks * 100) / total;
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

let percentage = function (marks, total) {
  return (marks * 100) / total;
}
// Your answer
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};

let percentage = function (marks, total) {
  return (marks * 100) / total;
}

```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
let percentage = function (marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
let percentage = function (marks, total) {
  return (marks * 100) / total;
}
```

```js
let percentage = (marks, total) => (marks * 100) / total;

let percentage = function (marks, total) {
  return (marks * 100) / total;
}
```

3. 
A function definition expression defines a JavaScript function, and the value of such an expression is the newly defined function. In a sense, a function definition expression is a “function literal” in the same way that an object initializer is an “object literal.” A function definition expression typically consists of the keyword function followed by a comma-separated list of zero or more identifiers (the parameter names) in parentheses and a block of JavaScript code (the function body) in curly braces. For example:

// This function returns the square of the value passed to it.
var square = function(x) { return x * x; };

4. Why is a function call an expression in JavaScript?

A function call expression is used to execute a specified function with the provided arguments.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3);  valid
five = add;  valid
five = five(10, 11); valid
five = function () {
  return 'Hello';
}; valid

all of them is valid as expresiion in first question as in second function reference is stored in third it will execute the function and add 10 +11 and in last same expression is being done
```

6. What is the difference between function definition and function call? Explain with an example.

function definition is the whole process of writing a function with keyword function and a name to the function whereas function call execute the function by function name and the required parameters.

7. What is the similarities between function definition and function call?

both requires function name as to define and to call also.

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!');
}

hello.user = 'Sam';  valid 
```

9. What is higher order function explain with an example.

Higher order functions are functions that operate on other functions, either by taking them as arguments or by returning them. In simple words, A Higher-Order function is a function that receives a function as an argument or returns the function as output.

10. Explain what is callback function. Why you can pass a function inside a function?

A callback function is a function that is passed as an argument to another function, to be “called back” at a later time. A function that accepts other functions as arguments is called a higher-order function, which contains the logic for when the callback function gets executed. It’s the combination of these two that allow us to extend our functionality.


For the given code below:

- re-write the code in ways that system will understand

For Example:

1.

```js
var username = 'Arya';
let brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// Declaration Phase
var username = undefined;
let brothers;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;

// Execution Phase

username = 'Arya';
brothers = ['John', 'Ryan', 'Bran'];

console.log(username, brothers[0]);

message = sayHello(username);
nextMessage = sayHello('Test');
```

2.

```js
console.log(username, numbers);

var username = 'Arya';
let number = 21;

function sayHello(name) {
  return `Hello ${name}`;
}

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
//declaration phase
var username = undefined;
let number;

function sayHello(name) {
  return `Hello ${name}`;
}

let message;
var nextMessage = undefined;
```

```js
// execution phase
console.log(username, numbers);

Uncaught ReferenceError: numbers is not defined;
```

3.

```js
console.log(username, numbers);
let username = 'Arya';
let number = 21;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message = sayHello(username);
var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase

let username;
let number;

let sayHello = function (name) {
  return `Hello ${name}`;
};

let message;
var nextMessage;
```

```js
// execution phase
console.log(username, numbers);
Uncaught ReferenceError: username is not defined;
```

4.

```js
let username = 'Arya';
console.log(username, numbers);

let number = 21;
let message = sayHello(username);

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = sayHello('Test');
```

<!-- Answer -->

```js
// declaration phase

let username;

let number;
let message;

let sayHello = function (name) {
  return `Hello ${name}`;
};

var nextMessage = undefined;
```

```js
// execution phase
let username = 'Arya';
console.log(username, numbers);

Uncaught ReferenceError: numbers is not defined;

```

5.

```js
console.log(name);
console.log(age);
var name = 'Lydia';
let age = 21;
```

<!-- Answer -->

```js
// declaration phase

var name = undefined;
let age;
```

```js
// execution phase
console.log(name); // 'Lydia'
console.log(age); // age isn't defined



```

6.

```js
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

sayHi();
```

<!-- Answer -->

```js
// declaration phase
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}

```
```js
// execution phase
function sayHi(name) {
  //declaration phase
  var name = undefined;
  let age;

  // execution phase

  console.log(name); // "lydia"
  console.log(age); // Cannot access 'age' before initialization

}

```

7.

```js
sayHi();
function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

<!-- Answer -->

```js
// declaration phase

function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
}
```

```js
// execution phase
sayHi();

function sayHi(name) {
  console.log(name);
  console.log(age); // Cannot access 'age' before initialization
  var name = 'Lydia';
  let age = 21;
}
```

8.

```js
sayHi();
let sayHi = function sayHi(name) {
  console.log(name);
  console.log(age);
  var name = 'Lydia';
  let age = 21;
};
```

<!-- Answer -->

```js
Uncaught ReferenceError: sayHi is not defined
```

9.

```js
let num1 = 21;
console.log(sum);
var sum = num1 + num2;
let num2 = 30;
```

<!-- Answer -->

```js
Uncaught ReferenceError: num2 is not defined
```

10.

```js
var num1 = 21;

let sum2 = addAgain(num1, num2, 4, 5, 6);

let add = (a, b, c, d, e) => {
  return a + b + c + d + e;
};
function addAgian(a, b) {
  return a + b;
}
let num2 = 200;

let sum = add(num1, num2, 4, 5, 6);
```

<!-- Answer -->

```js
VM14000:3 Uncaught ReferenceError: addAgain is not defined
```

11.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

let add = (a, b) => {
  return a + b;
};
```

<!-- Answer -->

```js
VM14030:3 Uncaught ReferenceError: add is not defined
```

12.

```js
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum = test(100);

function add(a, b) {
  return a + b;
}
```

<!-- Answer -->

```js
//declaration phase
function test(a) {
  let num1 = 21;
  return add(a, num1);
}

let sum;

function add(a, b) {
  return a + b;
}
```

```js
// execution phase
function test(a) {
  // declaration phase
  a= 100
  let num1;
  // execution phase
  num1 = 21;
  return add(100, 21);
}

let sum = test(100);

function add(100, 21) {

  return 100 + 21;
}
sum = 121
```


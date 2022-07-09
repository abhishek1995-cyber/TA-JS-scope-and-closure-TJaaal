Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya';
}
console.log(useranme); // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya';
}
console.log(useranme); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the  variable defined using const inside a block from outside.

The above code will throw an error `Reference Error username is not defined`.

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside the block and we can't access the  variable defined using let inside a block from outside.

The above code will throw an error `Reference Error username is not defined`.

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya';
}
console.log(useranme); // output
```
In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  var username = 'Arya';
}
console.log(useranme); 
```
Uncaught SyntaxError: Identifier 'username' has already been declared username has been declared already so we cant declare username using two variable

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
if (true) {
  let username = 'Arya';
}
console.log(useranme); // output
```
"john" as let is a block scoped and username john is derived globaly so it will print john.

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John';
function sayHello() {
  let username = 'Arya';
}
sayHello();
console.log(useranme); // output
```

john will be printe as first code will be declared and username will be empty after execution of code username will be john and execution of function say hello will be garbage collected as it is not expressed or stored in a variable 

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First');  it will print first 10 times value of i starting from 0 to 9 as it is printing inside loop so it will print one by one
}
console.log(i, 'Second');  it will print second 1 times value of i is 10  as it is consoled otside loop so it print the whole number of running loop at once
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First');  it will print first 10 times value of i starting from 0 to 9 as it is printing inside loop so it will print one by one
}
console.log(i, 'Second'); VM924:1 Uncaught ReferenceError: i is not defined as let is block scoped we cannot globally take value of i.
```


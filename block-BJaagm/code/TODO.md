1. What does thread of execution means in JavaScript?

JavaScript is not that fancy, it does two things. One, it goes through our code, line by line. There's a block of code we're gonna work through right now. It goes through it line by line, and does each of the line of code, they call this the thread of execution.

2. Where the JavaScript code gets executed?

Whenever the JavaScript engine receives a script file, it first creates a default Execution Context known as the Global Execution Context (GEC) . The GEC is the base/default Execution Context where all JavaScript code that is not inside of a function gets executed. For every JavaScript file, there can only be one GEC.

3. What does context means in Global Execution Context?

Whenever the JavaScript engine receives a script file, it first creates a default Execution Context known as the Global Execution Context (GEC)

4. When do you create a global execution context.

The Global Execution Context gets created when we load the JavaScript file, even when it is empty.

5. Execution context consists of what all things?

The Execution Context contains the code that's currently running, and everything that aids in its execution. During the Execution Context run-time, the specific code gets parsed by a parser, the variables and functions are stored in memory, executable byte-code gets generated, and the code gets executed.

6. What are the different types of execution context?

Global Execution Context (GEC)
Function Execution Context (FEC)

7. When global and function execution context gets created?

Whenever we execute JavaScript code, it creates a Global Execution Context (also knows as Base Execution Context).
When we invoke a function, a Function Execution Context gets created.

8. Function execution gets created during function execution or while declaring a function.

while declaring a function its creates a variable object. This process of storing variables and function declaration in memory prior to the execution of the code is known as Hoisting

9. Create a execution context diagram of the following code on your notebook. Take a screenshot/photo and store it in the folder named `img`. Use `![](./img/image-name.png)` to display it here.



```js
var user = "Arya";

function sayHello(){
  return `Hello ${user}`;
}

var userMsg = sayHello(user);
```

<!-- Put your image here -->

![](./img/image-name.jpg)

![](../IMG_8629.HEIC)

```js
var marks = 400;
var total = 500;

function getPercentage(amount, totalAmount){
  return (amount * 100) / totalAmount;
}

var percentageMarks = getPercentage(marks, total);
var percentageProfit = getPercentage(400, 200);
```

<!-- Put your image here -->

![](./img/image-name.jpg)

![](../IMG_8629.HEIC)


```js
var age = 21;

function customeMessage(userAge){
  if(userAge > 18){
    return `You are an adult`;
  }else {
    return `You are a kid`;
  }
}

var whoAmI = customeMessage(age);
var whoAmIAgain = customeMessage(12);
```

<!-- Put your image here -->

![](./img/image-name.jpg)

![](../IMG_8630.HEIC)


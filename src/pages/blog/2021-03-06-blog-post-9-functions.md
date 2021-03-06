---
templateKey: blog-post
title: "Blog Post #9 Functions"
date: 2021-03-06T21:34:50.916Z
description: Functions
featuredpost: false
featuredimage: /img/functions.png
tags:
  - "Blog #7"
---
![functions](/img/functions.png "functions")



Ways to define a function in JavaScript-

Function Declaration:

```javascript
// FUNCTION DECLARATION
function logSomething() {
  console.log('This is a function declaration');
}
```

Function Expression:

```javascript
// FUNCTION EXPRESSION
const someFunction = function () {
  console.log('This is a function expression');
};
const someArrowFunction = () => {
  console.log('This is a function expression as an arrow function');
};
```

Function Constructor:

```javascript
// FUNCTION CONSTRUCTOR
const constructorFunction = new Function('param', 'console.log(param)');

```

Immediately Invoked Function Expression:

```javascript
// IIFE
(function exampleIIFE(param) {
  if (param) {
    console.log('This is an Immediately Invoked Function Expression');
  }
})(true);

```

How to return a value from a function

```javascript
// RETURN A VALUE FROM A FUNCTION
function sum(num1, num2) {
    return num1 + num2
}
// Using return in the function statement returns the value.
```

How to accept a value into a function

```javascript
// RETURN A VALUE FROM A FUNCTION
function sum(num1, num2) {
    return num1 + num2
}
sum(100, 200)
// Passing the values to a function as arguments
// along with parameters specified allows for 
// accepting values into a function.
```

Callback Functions

A callback function is a function that accepts another function as a parameter.

The snippet below is an example of a callback function in action.

doesMath is a function that accepts 3 parameters. sum, num1 and num2.

In this scenario sum is a Callback function, and is accepted in doesMath because functions are objects in JavaScript. When I call doesMath with the 3 parameters defined I get the returned value from the sum function.

A use case for this is if you had separate functions for some mathematical operations and wanted to display all of them using the same parameters. like calling sum with the values in the example below you can easily call another function when passing it as an argument to a function.

```javascript
// RETURN A VALUE FROM A FUNCTION AS A CALLBACK FUNCTION
function sum(num1, num2) {
    return num1 + num2
}

const  doesMath = (sum, num1, num2) =>{
    return sum(num1, num2)
}

doesMath(sum, 500, 500)
```

What is a promise?

A Promise is a sort of placeholder for a value that may or may not be known at a given time in a piece of code. It represents the eventual success or failure of a process.

* How do they work?

  Promises have three states, Pending, Resolved or Rejected.

  When a promise is resolved it acts as a representation of the value it was previously the placeholder for. 
* When might you use on in your code? (Provide an example not using a built in method such as fetch())

  In our trivia app you could use a promise in a way to display a message after the game is over. The below function could be called when all the questions have been answered and after 1 second it would display a message that the game is over.

  ```javascript
  const message = new Promise((resolve, reject) => {
    setTimeout(() => {
      resolve('Game is over, Play Again?');
    }, 1000);
  });
  ```
* What is the async, await syntax? How does it work?

  async and async await are designed to make working with promises more readable.

  writing the above function with async in front of it makes it return an eventually resolved promise. The goal of async await is to make it easier to know when a promise has been resolved and create a more readable block.

  ```javascript
  asyn const message = () => {
   const await afterTimeout =  setTimeout(() => {
      resolve('Game is over, Play Again?');
    }, 1000);
  });
  ```
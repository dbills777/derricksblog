---
templateKey: blog-post
title: "Blog post #3 - Functions, Objects, and Arrays"
date: 2020-09-04T22:43:53.742Z
description: A Bit About Functions
featuredpost: true
featuredimage: /img/functions.png
tags:
  - Functions Objects Arrays
---
**Post 3 - Functions, Objects, and Arrays**

**What are functions in Javascript?**

In short, functions in javascript are tools we as developers can use to define a block of code and have the ability to reuse that code and repeat its processes as little or as many times as we need.

Before we can use a function in our application we must first be able to define one.

**Function Declaration**

```javascript
function findBook(array, title){
    for(let i = 0; i < arr.length; i++){
      if(arr[i] === name){
        return `${name} is a book in the array!`
      }
    }
    return `${name} is not in the array`
  }

  let myBooks = ['A Storm of Swords', 'The Hobbit',
                 'Design of Everyday Things']

  findPerson(myFriends, 'The Hobbit') 
// outputs `The Hobbit is a book in the array`
```

In the code block above we have "declared" a function, this is done with the function keyword and following it up with the function name "findBook". Next we can add what parameters if any we want to be available to the function, in this case we pass it an array and a title. This is because our functions job is to find a book in a list of books. 

**Function Expression**

```javascript
let addOne = function AddOne(num){
    return `${num} +1`
  }

// below the function is called and 10 is passed in as the num argument
addOne(10)
// outputs `11`
```

In the code block above we have "defined" a function expression, this is slightly different that the named function as it stores the function in the variable name that we provide. One of the main differences that these two types of functions have is that a function declaration is "hoisted" to the top of our code at runtime and a function expression is not. This means we could create a function declaration at the bottom of our code and call a function at the top and it would execute that function. if it is a function Expression or an Arrow function we would receive an error of "not defined".

**Arrow Functions**

```javascript
let addOne = function AddOne(num){
    return 'num +1'
  }
// below the function is called and 10 is passed in as the num argument
addOne(10)
// outputs '11'
// Arrow function implied return with no brackets
let addTwo = num => num + 2

// Arrow function with return statement
let addTwo = num =>{
  return num + 2
}
addTwo(20)
//ouputs '22'
```

In the code block above we have "defined" an Arrow Function this is nearly identical in practice to the addOne() function shown above it. Although there are some differences. If the function declaration and the return statement are on one line we can right it as shown above on line 9. On line 11 it is written with an included return statement. This is how it would be written for a complex function body that can not all be contained on one line. They also handle the binding of the "This" keyword differently than other functions, but that will be covered later.

**Callback Function**

```javascript
const result = filter([3, 6, 1, 10], function greaterThanFive(item) {
  return item > 5;
});
 
console.log(result);
// [6, 10]
```

In this example our named function "result" contains a filter method that receives two arguments. The first argument is an array that it wishes to perform a given operation on, and a function that is to be permed on the given array. The process for this example is filter passes the array of numbers and calls the 2nd parameter, the function greaterThanFive(item). The array is represented by the item parameter and the operation is performed on the array. In this example it filters out only numbers that are greater than five. The real advantage is that this type of function will continue to run until it has processed the entire array or other piece of data that it is working on with a single function call.

**Promises**

```javascript

const delay = time => new Promise((resolve) => setTimeout(resolve, time));

delay(3000).then(() => console.log('This Promise resolved after '+ time+'ms'));
//output 'This Promise resolved after 3000ms'
```

Without getting into the depths of promises it is a concept that a specific function will perform an operation, and upon that resolution it is said that the promise has been resolved. In the code example able the promise is resolved after the delay time has lapsed. at that point it will .then continue on with its other operations. This gives a program time to receive or complete a task and to be "ready" for the output from the promise. 

**Objects**

A Javascript object is a primitive data type that is used to structure our data in an organized way for use in our applications. here is a quick example of an object structure

```javascript
let person = { 
                firstName: "Gus", 
                lastName: "Fring", 
                age: 51, 
                getFullName: function () { 
                        return this.firstName + ' ' + this.lastName 
                }
            }; 
```

in this example we are using the Object Literal syntax in defining our object. Objects are made up of key value pairs and can accept a huge amount of data types in the value pairs it accepts. Above we have a person object with multiple keys and values. from strings to numbers and even functions can be added to an object. This allows for better systematic grouping of items that belong together like details about a specific person in this case.

**Arrays**

A Javascript object is a primitive data type that is used to structure our data as a type of list grouping for later use in our applications. 

```javascript
let people = ['Cersei', 'Tyrion', 'Tywin', 'Jaime']


for (const person of people) {
  console.log(person);
}

// expected output: "Cersei"
// expected output: "Tyrion"
// expected output: "Tywin"
// expected output: "Jaime"
```

Arrays are declared much like any variable and designated with the outer \[]'s. They can contain many data types as well as nested arrays. one of the great benefits of arrays are how easy it is to loop through them. 

in addition to the for loop outlined at the beginning of the article we can also use A for.... of loop. It is worth a look into all the different loops and methods that are available as part of javascript to work with arrays and objects. 

This week I also learned some great points about data types in javascript and the pitfalls that can be avoided when paying close attention to them in our code. Noticing problems that can arise from improper use of data types early on in our code can alleviate many issues later down the development line.
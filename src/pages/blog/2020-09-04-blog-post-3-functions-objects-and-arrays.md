---
templateKey: blog-post
title: "Blog post #3 - Functions, Objects, and Arrays"
date: 2020-09-04T22:00:53.265Z
description: A Bit About Functions
featuredpost: false
featuredimage: /img/products-grid2.jpg
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

* How do you use promises in functions?
* What are objects in Javascript

  * How are they used and defined?
  * How do you loop through an object?
* What are Arrays in Javascript?

  * How are they used and defined?
  * What are 2 ways to loop through an array?
* Write about at least one other thing you learned this week.

Code examples are a great way to explain these questions.

Please turn in a URL to your post for this assignment.

Lastly, post a link to this post in MS Teams in the channel called **F.O.A Blog Post.** Please comment on at least 2 other posts in Teams.

What did your classmates do well? What did you learn?
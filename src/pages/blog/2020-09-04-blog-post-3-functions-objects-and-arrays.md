---
templateKey: blog-post
title: "Blog post #4 - Advanced Functions"
date: 2020-09-02T22:00:53.265Z
description: ________________________________
featuredpost: false
featuredimage: /img/damian-zaleski-ryyr-k3ysqg-unsplash.jpg
tags:
  - Advanced Functions
---
**Post 3 - Advanced Functions**

* What is recursion?

  Recursion is a technique for iterating over an operation by having a function call itself repeatedly until it arrives at a desired case (Base Case or Exit Case). 
* What are Scopes and Closures in Javascript?

  Scope is a way to manage the availability of variables and their values in functions or from the place they were originally assigned. They are important because they allow us to encapsulate our code, this keeps variable local or private to the items that are reliant upon them. Scoping also guards against accidental reassignment or mutation of variables.

  A closure is created every time a function is created, this allows an enclosed function to have reference to items that are outside of it. this is important if you want to access a value that is declared somewhere in the lexical environment you are allowed to.

  Having a strong understanding of what is and what isn't available to a function or to other parts of an application is important. It can save needing to repeat code and also protect against having bugs or items that are meant for private use of a function being exposed to other parts of our code.
* What is the Spread Operator?

  ```javascript
  arr1 = [1,2,3,4]
  arr2 = [3,4,5,6]
  //spread operate will combine the two arrays into one 
  const combined = [...arr1, ...arr2]
  ```

  The spread operator allows for an item that is iterable to be expanded in places where arguments are passed. My favorite use is to use it for array duplication as it is one of the most simple ways to do this. it also is great for combining two arrays into a new single array.

This week I learned about recursion and how it can be used in data structures. And how it can be used to "loop" through objects.
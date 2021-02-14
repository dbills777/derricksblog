---
templateKey: blog-post
title: "Blog Post #6 TypeScript"
date: 2021-02-14T01:02:40.531Z
description: TypeScript
featuredpost: false
featuredimage: /img/testing.png
tags:
  - "Blog #4"
---
![tdd](/img/testing.png "tdd")

*   **Post 4 - Unit Testing**

  * What is unit testing?

    Unit testing is systematically writing test cases for a small chunk or unit of code, for a small portion of the overall functionality of that piece of code. Only once the small piece of code passes the unit test do you begin on with the next function that the unit needs to accomplish.  
  * What is test driven development?

    Test driven development is a method of testing and developing in a pattern of; Testing, Writing part of the code solution, testing again, writing a new test and refactoring the code. This loop allows for small chunks of code to be developed in a way that encapsulates them from the overall application that is being developed. In this scenario, code is written only to accomplish what the test says it should do. 
  * Why would you practice test driven development?

    A good use case for this development strategy is a highly computational small function. If you had many pieces of data to calculate manipulate and display in a relational way, TDD is a perfect strategy for breaking the problem down into small easy to manage pieces.
  * What are the advantages and disadvantages of test driven development?

    One advantaged to test driven development is that by the time the product is complete the testing has also been done. This eliminates the need to go back and test the code later. 

    It is also makes quick work of "simple" mistakes. Writing small chunks to accomplish a given test can help to catch small errors that may otherwise be overlooked. 

    A few downsides of Testing are that the tools needed to complete the testing need to be maintained. this maintenance requires time and manpower. It is also something that takes a bit of onboarding to really accomplish. The whole team needs to buy in for it to truly be successful. 
  * What is a unit?

    A unit is a sort of vague term. Possibly it is vague intentionally, but it can be interpreted as a small "unit" of an application that is responsible for one specific task. It can be complex in itself, but keeping it isolated from other operations and dependencies keeps this unit type structure.
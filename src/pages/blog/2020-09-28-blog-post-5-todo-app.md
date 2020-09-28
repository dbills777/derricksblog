---
templateKey: blog-post
title: "Blog post #5 -Todo App"
date: 2020-09-28T01:21:40.447Z
description: ________________________________
featuredpost: false
featuredimage: /img/screen-shot-2020-09-27-at-7.18.45-pm.png
tags:
  - TodoApp
---
My Todo app gives the option of entering a Todo with or without a category typed in. If no category is entered it assigns it a category of "No category Entered".  after entering a new Todo Item it is placed in the top list on the left (light blue color) and also the Category section(red color ) on the right. If the todo is marked as completed it moves from the todo category to the completed(green color) section on the left bottom. 

The overview Category section also marks the completed todos as such and has some hover effects when the user hovers over them, it magnifies the todo for better viewing. I designed it this way to have a good overall feel of the flow of the data when an item is entered or deleted. as well as when they are marked off as complete. the changing of a todos position to the two main lists helps to see the flow. 

![](/img/screen-shot-2020-09-27-at-7.18.45-pm.png)

Some of biggest challenges I had were the deleting and moving items to different lists at the same time. I tried to solve this by having the items be rendered into each list based on the condition of completed being true. This ended up working great and fulfilled the needs of the application. 

If I were to do it all over again I would spend a good amount of time on picking an layout that displays the data in a more efficient way. either only using the final red category list to handle all the functionality or a completely different design altogether. 

Overall I think if i did made this application five different times I would have five different applications that all accomplished the goal, just in very different ways. I would also work on structuring it into more functional components or even class components with static methods to complete each manipulation on the data as needed.
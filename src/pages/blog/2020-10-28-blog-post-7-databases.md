---
templateKey: blog-post
title: "Blog post #8 Todo App Backend"
date: 2020-10-28T19:00:52.385Z
description: ________________________________
featuredpost: false
featuredimage: /img/screen-shot-2020-10-28-at-1.02.34-pm.png
tags:
  - Node
---
![](/img/screen-shot-2020-10-28-at-1.02.34-pm.png)



* How did you design/architect your your app and server?

  My application relies heavily on the front end to handle display using sorting, filtering, and mapping of the todos returned by the database. The server endpoints are only needed to add, mark complete, delete. my front end designed allowed for a simpler integration for the front and back end.

  My application uses the express.static(public) method of displaying the front end files to the web, And uses an express and mongoose server to handle endpoint behavior.

  * How did the front end connect to the backend?

    It connects to the mongoDB using mongoose and that handles all of the necessary endpoints to Edit and display the data as needed.

    I used express and mongoose to connect to my mongoDB database to store and manipulate the data as needed by my front end application.
* Why did you choose the design you did?

  When I was designing the original todo I wanted it to be able to handle most of the functionality from one single array of objects. This design allowed me to quickly implement the backend fetch() calls and make subsequent calls as needed to fill my 3 display sections.
* How did you model you data and why?

  My data model was fairly simple, I only require a Todo with no relations to fully handle all the required endpoints. It relies on the front end to choose how to filter and display the data rather than the relations in the database.
* Why is documentation important?

  Documentation is important to me because often times I forget most of the necessary information I had in my head at the time that I wrote it. Creating good documentation allows me to quickly give myself a reference of what my thought process was at the time of creation. This is meant to help me to remember what function each documented piece of code performs. This becomes vital when revisiting an older piece of code that I have previously written.
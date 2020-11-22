---
templateKey: blog-post
title: "Blog post #6 -NodeJS"
date: 2020-10-10T22:31:39.385Z
description: ________________________________
featuredpost: false
featuredimage: /img/node.png
tags:
  - Node
---
![](/img/node.png)

* What is Node JS?

Node JS is a runtime environment that executes JavaScript outside of a Web Browser. It allows scripts to be run server side to produce dynamic web page content before the page is sent to the user’s web browser.

* When do you use Node? Name 4 use cases and describe them.

Chat -receiving and forwarding messages with Node and something like express make great use of using the processing power of the server vs the client. With many requests coming in to the server in a chat scenario Node can quickly route and update a user's client as the updates appear.

Streaming Style Applications - If an application has to upload and process data quickly, Node's ability to process it while it is continuously being uploaded to the server is a great ability. It is able to process chunks of data without needing to wait for the entire file to be uploaded.

Rest API’s - Rest API’s rely on HTTP protocol’s this high demand of needed to access data through HTTP requests to, say for example a database, is something that Node does in a quick and easy fashion.

Command Line Tools - building scripts for later use and reuse increases productivity and streamlines the development process. We can create packages and share them, update/manage with various Node libraries and frameworks.

* What are some ways that Node differs from JS in the browser?

There is no DOM in a NodeJS environment, The Global Object in a browser is the Window object, in NodeJS the Global object is the module itself. This means that all the types available to the window object are not available in node JS. Node also gives access to the system that the browser does not have, for example the fs or file system allows NodeJS to write, read, update, delete files on a local machine or server.

* What is Express JS?

Express is a web framework for NodeJS. It has many API’s that are prebuilt and very efficient for working with server side operations. This saves developers time and also easier to write code than the standard NodeJS approach.

Express is very useful at quickly implementing some of Node's best features, rather than writing all the NodeJS code from scratch it has a large framework of items that solve these problems in a quick and easy manner.

* Why would a developer choose to use a Templating Engine?

Templating Engines allow us to replace variables in static template files at runtime, these files are then sent to the client and used to build the webpage based on the dynamic data, developers use this to quickly render data from a server that is dynamic.

* What Templating Engine did you choose and why?

I chose to use ejs, due to its large weekly download numbers on npm, there were many to choose from, so I simply had to just pick one and move on. Overall the syntax made sense to me and the documentation was great.
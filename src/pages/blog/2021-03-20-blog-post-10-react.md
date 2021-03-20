---
templateKey: blog-post
title: "Blog Post #10 React"
date: 2021-03-20T22:13:22.420Z
description: ReactJS
featuredpost: false
featuredimage: /img/react.jpeg
tags:
  - React
---
![react](/img/react.jpeg "ReactJS")



React is a JavaScript Library for building user interfaces. The prime task that react was created to solve was interactivity in websites, and how to run interactive elements into a continuously reactive UI. The elements of a website that a user interacts with require more complex solutions to handle those interactions. for this reason FaceBook and and their JavaScript Development Team Created the React Library.



State is the term used for the current values of an application at a given time. for example, logged in could is a state that an application could have, as well as items in cart. State is simply the current values of the application that need to be kept track of in order to offer interactivity to a User

State management is often done with the passing of props, libraries, or by the newer context api that is part of the core react library. any of these methods allow for developers to share the current state of an application with other parts of the application that may need to change or that rely on them.  These actions are sometimes called "lifting up state"

JavaScript now offers a Class like object to more closely related to lower level programming languages. This new change to the core of javascript prompted the early version of react to be primarily based of a class based implementation. This also meant that initially only class based components in react could handle and applications state. Later, they introduced Hooks to the library and added state capabilities to functional components. A class based component renders an element to the DOM and operates in a similar way to a class constructor in the base javaScript manner. 

Functional components are simply JavaScript functions that return some form of JSX, the returned js is then what is used to create the UI

The use of class or functional components is mostly a matter of personal choice by the designer of the system that is being created. currently a shift has been made to write React applications almost exclusively with functional components. This approach makes it more readable and translatatebly for those coming from other areas of Javascript.

React uses JavaScript Extension or JSX to write React applications. this extension to javascript allows for a simpler syntax for writing elements that will populate the virtual DOM and later be used as the basis for the real browser DOM.
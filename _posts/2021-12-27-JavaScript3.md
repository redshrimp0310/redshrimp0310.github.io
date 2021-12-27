---
title:  "Function(2) in JavaScript"
excerpt: "Basics(2) of function in JavaScript"

categories:
  - JavaScript
tags:
  - [TIL, function, JavaScript]

toc: true
toc_sticky: true
 
date: 2021-12-27
last_modified_at: 2021-12-27
---
## FUNCTION

### Function that return a function
As described in the last post, Function is treated as a first class object. So, Function is able to return a function. 

![JS](/img/JavaScript/JS3/2021-12-27-JS3-1.jpg)

### Arguments Object

Unlike C language, an error does not occur in JavaScript when passing more or less than two arguments as below. 

![JS](/img/JavaScript/JS3/2021-12-27-JS3-2.jpg)

Arguments Object is an array-like object passed into the function to represent the list of arguments that are passed in when a function is invoked.

![JS](/img/JavaScript/JS3/2021-12-27-JS3-3.jpg)

Arguments Object is beneficial when we create a function with an unknown number of arguments. 

![JS](/img/JavaScript/JS3/2021-12-27-JS3-4.jpg)

### Function Invocation Patterns & This Binding

'This' argument is also passed into the function as well as Arguments object when a Function is called.  
  
When a Method is invoked, 'This' used in the Method refers to an object that called that method.

![JS](/img/JavaScript/JS3/2021-12-27-JS3-5.jpg)

a Global variable is actually a property of a Global Object.  

![JS](/img/JavaScript/JS3/2021-12-27-JS3-6.jpg)

When a Function is invoked, 'This' used in the Function refers to a Global Object.  

![JS](/img/JavaScript/JS3/2021-12-27-JS3-7.jpg)

Same 'this' binding rule applies to when a Inner Function is invoked.

![JS](/img/JavaScript/JS3/2021-12-27-JS3-8.jpg)

![JS](/img/JavaScript/JS3/2021-12-27-JS3-9.jpg)

Code can be amended as below to overcome that 'this' refers to a Global object.

![JS](/img/JavaScript/JS3/2021-12-27-JS3-10.jpg)

![JS](/img/JavaScript/JS3/2021-12-27-JS3-11.jpg)

'this' inside a constructor function works differently when it's called.

![JS](/img/JavaScript/JS3/2021-12-27-JS3-12.jpg)

![JS](/img/JavaScript/JS3/2021-12-27-JS3-13.jpg)

When a constructor function is invoked without 'new' or a normal function is called with 'new', an error occurs. That's because 'this' inside a constructor function refers to a created empty object while 'this' inside a normal function refer to a 'Window' Global object.

![JS](/img/JavaScript/JS3/2021-12-27-JS3-14.jpg)

Naming convention that the first letter of function name is capitalized is strongly recommended for a constructor function.













## REFERENCE 
* 송형주,고현준 Inside JavaScipt 한빛미디어(2017)
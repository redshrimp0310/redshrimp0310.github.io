---
title:  "FUNCTION in JavaScript"
excerpt: "Basics of FUNCTION in JavaScript"

categories:
  - JavaScript
tags:
  - [TIL, FUNCTION, JavaScript]

toc: true
toc_sticky: true
 
date: 2021-12-22
last_modified_at: 2021-12-22
---
### FUNCTION
Function is a block of code designed to perform a certain task and anonymous function is a function that does not have any name associated with it. When creating a function, we don't declare parameter types.

* There are generally there ways of creating a function in JavaScript.

1. Function Statement

Function literal is used.
Function name MUST be declared. 
Semicolons after function declarations are not necessary.
![JS](/img/JavaScript/js2/2021-12-22-JS2-1.jpg)

2. Fucntion Expression

Function literal is used.
Function name is optional.
Semicolons after function declarations are not necessary.
The funciton is stored into a variable.
This variable is reference variable.

![JS](/img/JavaScript/js2/2021-12-22-JS2-2.jpg)

When we declare the name of function and assign the function to a variable, we can't access the function by calling the funcion name. Instead, we need to call a variable's name.

![JS](/img/JavaScript/js2/2021-12-22-JS2-3.jpg)

The below function is internally amended by JavaScript Engine.

![JS](/img/JavaScript/js2/2021-12-22-JS2-4.jpg)
![JS](/img/JavaScript/js2/2021-12-22-JS2-5.jpg)

The function name can be called as below.

![JS](/img/JavaScript/js2/2021-12-22-JS2-6.jpg)

3. Function() Constructor 

Function statement and function expression is the process of the simplified procedure of creating function by using of Function() constructor.

Syntax :
new Function(arg1, ... , argN, functionBody)

* Function Hoisting

Hoisting can allow functions to be used before they are declared in the code.

![JS](/img/JavaScript/js2/2021-12-22-JS2-7.jpg)

It can lead to the unexpected errors and is not normally recommended.

![JS](/img/JavaScript/js2/2021-12-22-JS2-8.jpg)

* Function is also an ojbect. It can have properties.

![JS](/img/JavaScript/js2/2021-12-22-JS2-9.jpg)
![JS](/img/JavaScript/js2/2021-12-22-JS2-10.jpg)

* Function in JavaScript is called first class object due to the following reasons:

1. Can be created by literal.
2. Can be assigned to variable, element of array, and property of object.

![JS](/img/JavaScript/js2/2021-12-22-JS2-11.jpg)

3. Can be used as an argument of function.

![JS](/img/JavaScript/js2/2021-12-22-JS2-12.jpg)

4. Can be used as a return value of function.

![JS](/img/JavaScript/js2/2021-12-22-JS2-13.jpg)

5. Property can be created and assigned dynamically.

* There are additional standard properties defined into a function object such as arguments, caller, lengh, etc.

![JS](/img/JavaScript/js2/2021-12-22-JS2-14.jpg)

Length property

![JS](/img/JavaScript/js2/2021-12-22-JS2-15.jpg)

* Callback Function

Callback function is a function passed as an argument into another function

* Immediate Function

Immediate function is a function that enables you to execute a function as soon as defined.

![JS](/img/JavaScript/js2/2021-12-22-JS2-16.jpg)

* Inner Function

![JS](/img/JavaScript/js2/2021-12-22-JS2-17.jpg)

* Closure

This is a feature where an inner function has an access to the outer function's variables.

![JS](/img/JavaScript/js2/2021-12-22-JS2-18.jpg)


### REFERENCE 
* 송형주,고현준 Inside JavaScipt 한빛미디어(2017)
* https://www.w3schools.com/js/js_functions.asp
* https://developer.mozilla.org/en-US/docs/Glossary/Hoisting
* https://developer.mozilla.org/en-US/docs/Glossary/Callback_function
* https://www.oreilly.com/library/view/javascript-patterns/9781449399115/ch04.html
* https://medium.com/@prashantramnyc/javascript-closures-simplified-d0d23fa06ba4





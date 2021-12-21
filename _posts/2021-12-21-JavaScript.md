---
title:  "Array and Operator in JavaScript"
excerpt: "Basics of array and operator in JavaScript"

categories:
  - JavaScript
tags:
  - [TIL, Array, JavaScript]

toc: true
toc_sticky: true
 
date: 2021-12-21
last_modified_at: 2021-12-21
---
### ARRAY
* Arrays are list-like objects and can store multiple data types. An array literal is a list of array elements, enclosed in a pair of square brackets '[]'.

![JS](/img/JavaScript/2021-12-21-JS1-1.jpg)
- - -
* Accessing an Array item using the index position.

![JS](/img/JavaScript/2021-12-21-JS1-2.jpg)
- - -
* When adding a property to an array, if that index is outside the bounds of the array, the array's length property is updated accordingly.

![JS](/img/JavaScript/2021-12-21-JS1-3.jpg)
- - -
* If we set the length, the elements of the array will be deleted to the value of the length property set.

![JS](/img/JavaScript/2021-12-21-JS1-4.jpg)
- - -
* When we create an object by using object literal, the prototype(the parent of an object) of 'the object' is Object.prototype. However, the prototype of Array is Array.prototype and also Object.prototype. It indicates that Array can use the methods belong to both Array.prototype and Object.prototype.

* We can add a property as below.

![JS](/img/JavaScript/2021-12-21-JS1-5.jpg)
- - -
* When deleting the element of array, delete can be used but the length of the array will NOT be updated accordingly. So, we can use Splice() array method instead to update the length as well. 

![JS](/img/JavaScript/2021-12-21-JS1-6.jpg)
- - -
* When an array is created, we normally use an array literal but it's just the process of the simplified procedures of creating an array by using Array() constructor.

![JS](/img/JavaScript/2021-12-21-JS1-7.jpg)
- - -
*  An array-like object is an object that has indexed access to the elements and a non-negative length property to know the number of elements. It doesn't have any of the Array methods like, push, pop, join, map, etc.

![JS](/img/JavaScript/2021-12-21-JS1-8.jpg)
![JS](/img/JavaScript/2021-12-21-JS1-9.jpg)
- - -
* There are standard methods for number, string, and boolean. When the method is called, the value is temporarily converted to an object and re-converted back to the value when completed. 

![JS](/img/JavaScript/2021-12-21-JS1-10.jpg)
- - -
### OPERATOR
* '+' operator

![JS](/img/JavaScript/2021-12-21-JS1-11.jpg)
- - -
* typeof operator
null & array : object, function : function
- - -
* !! operator
It returns true if non-zero. Otherwise, returns false.

when Object is empty, '!!' operator returns true. On the other hands, when String is empty, it returns false.

![JS](/img/JavaScript/2021-12-21-JS1-12.jpg)
- - -
### REFERENCE 
* 송형주,고현준 Inside JavaScipt 한빛미디어(2017)
* https://www.w3resource.com/javascript/variables-literals/literals.php
* https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array
* https://medium.com/dev-proto/javascript-reducing-array-elements-using-the-length-property-6278e1a20afc
* https://www.capscode.in/blog/what-is-array-like-object-in-javascript
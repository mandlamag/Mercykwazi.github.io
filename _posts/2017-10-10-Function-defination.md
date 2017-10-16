---
layout: 
title:  "Function defination"
date:   2017-10-10 09:40
categories: 
---
It is important to know how to define a function in javascript so that you can understand that what the function is doing.

JavaScript functions are defined with the function keyword.
You can use a function declaration or a function expression.

Function declarations and Function expression

Function Declaration
A Function Declaration defines a named function variable without requiring variable assignment.
Function Declarations occur as standalone constructs and cannot be nested within non-function blocks.
It’s helpful to think of them as siblings of Variable Declarations,Just as Variable Declarations must start with “var”, 
Function Declarations must begin with “function”.
example:
	
function bar() {
    return 3;
}
 The function name is visible within it’s scope and the scope of it’s parent.
 Which is  a good thing because otherwise it would be unreachable.
 function bar() {
    return 3;
 }
 
bar() //3
bar  //function
Function Expression?

A Function Expression defines a function as a part of a larger expression syntax (typically a variable assignment ).
Functions defined via Functions Expressions can be named or anonymous.
Function Expressions must not start with “function” 

example:
	
(anonymous function expression)
var a = function() {
    return 3;
}
 
(named function expression)
var a = function bar() {
    return 3;
}
 
(self invoking function expression)
(function sayHello() {
    console.log("hello!");
})();



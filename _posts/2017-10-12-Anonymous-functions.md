---
layout: 
title:  "Anonymous function"
date:   2017-10-12 09:40
categories: 
---
Anonymous functions you always came across them in most code,understanding how they work is very important

 An anonymous function is a function that is not stored in a program file, but is associated with a variable whose data type is function_handle.
 Anonymous functions can accept inputs and return outputs, just as standard functions do,However, they can contain only a single executable statement.
 It is a function that is  not bound to an identifier.
 They are most of the time :
       
    -arguments being passed to higher-order functions, 

    -used for constructing the result of a higher-order function that needs to return a function.

 If the function is only used once,  an anonymous function may be the best solution to be used  than using a named function.

  Anonymous functions are a form of nested function.

  They  allow the access to variables in the scope of the containing function (non-local variables).

  Their use:
  Anonymous functions can be used for containing functionality that need not be named and possibly for short-term use. 

  Using them is never the only way to solve a problem; each anonymous function could instead be defined as a named function and called by name.

---
layout: 
title:  "reduce-function"
date:   2018-01-12 09:40
categories: 
---
# Reduce
One of the most used javascrip methods is the reduce method.
It is a method  that applies a function against an accumulator and each element in the array (from left to right) to reduce it to a single value. 
This method is mostly used when you have two arrays and you want to add the total of both these arrays.
The method takes four arguments,which are the callback and intial value
## callback
This function is called to execute all the elements in the array.
The callback also takes 4 arguments which are:
#### Initial value
This value is the first value to be executed when a callback is executing,it is therefore important to specify this value because when the value is not specified the first value in the array will became this value,If the array is empty an erro will be returned.
#### currentValue
This the  current element being processed in the array.
#### currentIndex
The index of the current element being processed in the array,this index stars at 0 when it is specified or provided and if not it will starts at index.
#### array
This is an array,which  reduce was called upon.


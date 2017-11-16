---
Layout: 
Title: "Finders keepers"
date:   2017-11-16  09:40
categories: 
---
# Finders keepers

## Theory
When I was solving this problem I did not strangle that much I found  the problem approachable.

## The problem
This activity required that Given a function with two arguments an Array and a  function I must:

Create a function that looks through an array (first argument)

The function must return the first element in the array that passes a truth test (second argument).

## My approach
### Created a function
Inside my first function I created another function that validates the argument passed in it.

In that function I gave it a conditional statement.

In the if statement I said whatever value is passed in as an argument it must be devisable by 2 and leave zero as a remainder.

And if thats the case the value passed in must be returned. 

## filter
I then used the filter method to filter though my array and called in my function

The filter method will go in the array and check which number in the array is devisable by two and leaves the remainder 0;
I then return the array but in my return statement I specified that It should retain the first value by indicating with array index 0

## Conclusion 
My function was now working.
In this activity I created another function which was not necessary.
I could have used th given function as an argument but I did this so that I get familiar with  writing two functions,
and also calling the function that I have created in the other function.
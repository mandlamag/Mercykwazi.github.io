---
layout: 
title:  "Sorted Union "
date:   2017-11-02 09:40
categories: 
---
Today in freeCodeCamp I came across an interesting challenge that I will share how I solved the problem.

The Challenge:

Was to write a function that takes two or more arrays and returns a new array;
of unique values in the order of the original provided arrays.

What was given:

A function with a name that had one parameter;

My approach:

When I first read the problem I decided to break it down in my own
logical understanding without writing the code down.

First-step:Change the arguments into an array.

In my function that was already provided for me I created a variable that I assigned my arguments
to it using the Array.from(arguments)method.This method turns what ever argument you will pass to the function to an array.
I used this method so that no-matter the number of arguments can pass,those arguments will be passed into  a single array.

Second-step:Creating an empty array.

I created a new variable which assigned it to an empty array.
I was going to use the variable at a latter stage because I already had a picture on how my function would look like at the end.

Third-step:Using a reduce method

In this step I first created a new variable which I assigned it to
my first variable that contained the argument that was changed to an array.
When I changed my arguments to an array I had 1 array that contained different arrays inside it,
I then used the reduce method  to executes a my function for each value of the array.
In my reduce function I used two parameters.I then used the concat method so that the returned value can be a single array containing all the values that were in the different arrays.

Forth-step:Using a for-loop and If-statement

I then used a for-loop to iterate my new array that was generated using the reduce method.
Inside my for-loop I had an if-statement that said that if that empty array that I created in the beginning its index i was not    strictly equal to -1  whatever the index is must be pushed in that array.
Then I returned the empty array which now contained the new array without any duplication.
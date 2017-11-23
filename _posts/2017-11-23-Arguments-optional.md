---
Layout: 
Title: "Arguments Optional "
date:   2017-11-23 09:40
categories: 
---
# Arguments optional
## My story
When it came to solve this activity it was quite challenging.
It took me a very long time to understand what the problem was requiring.
So I slowly broke it down to smaller pieces.

## The problem
Create a function that sums two arguments together.
If only one argument is provided, then return a function that expects one argument and returns the sum.

## My approach 
## My rules 
I first broke down my problem in the following steps:

With the given function it did not not have parameters,so I needed to add parameters for the given function.

I needed a new function that will validate whether the given is a number or not.

I also need another function that will be returned if one argument is given.

## first-step
In the given function I added two  parameters so that I can be able to carter for two arguments.
## second-step
Still in the first function,I created a function that will validate whether the passed argument is a number or not,
if it is a number it should return the boolean true otherwise false.
## third-step
I then added conditional statements inside my first function.
The first one called my validation function and said if the first argument in my main function is not a number type it should return undefined 
eg(!isNum(num1)) {
        return undefined;
    }
The second if statement said that if both my arguments in my main function they are a number type then the sum of the two should be returned.
## forth-step

I then used a conditional statement  that said that if it happens that my second argument is not defined,
Within that conditional statement I created a new function that takes one value as an argument.
So I said that if it is not the second argument then the sum of the first argument of my main function and the value of the last function 
must be returned.

## Conclusion
Now that my function was now catering for all the possible scenario.
My activity was now compete.
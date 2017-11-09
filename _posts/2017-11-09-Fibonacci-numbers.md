---
Layout: 
Title: "Sum All Odd Fibonacci Numbers "
date:   2017-11-09  09:40
categories: 
---
## Sum All odd Fibonacci Numbers
## Requirements 
This activity that I did today in free-code camp required the following things:

When you are given a positive integer num, return the sum of all odd Fibonacci numbers that are less than or equal to num.
## what was given.

I was told that the first 2 numbers on the sequence were [1,1];

## My approach
## first-step
I first had to understand what a Fibonacci sequence was.

A  Fibonacci sequence is a series of numbers where a number is found by adding up the two numbers before it.

## second-step
When I had found out how to get a fibonacci sequence from its definition I figured out a pattern in my heard how I was going to solve the problem.

From the definition I knew that to get the next number I must the previous one together with the current one.

so I decided to: 

create a variable  called previousNumber and I assigned it to 0;

create another variable called currentNumber and  I assigned it to 1;

create another variable that wil handle the results;

## third-step:While-loop
I decided to use a while-loop and specified a condition that when-ever a value is passed it should not be less-than or equal to the currentNum;

The while loop will iterate through the given condition until it breaks where i will be greater than num;

## forth-step:if-statement
After using a while-loop I nested it with an if statement that specified that if my currentNub's reminder is not equal to 0 then  add that number to results.

I then closed my if statement.

## fifth-step:
Still inside my while-loop I then assigned currentNub to my previous number.

I then said that my previous number was equal to currentNum minus the previous number.

## Conclusion
Then I returned results.

Now my function was returning what was the sum of all odd Fibonacci numbers that are less than or equal to num. 



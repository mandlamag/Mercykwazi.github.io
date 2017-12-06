---
Layout: 
Title: "Symmetric Difference"
date:   2017-12-05 09:40
categories: 
---
# Symmetric Difference
## My story
Yesterday I tried solving this problem but I wasn't successful, today I managed to solve this problem.
I found this activity very challenging, It took  me a lot of time to understand what the problem wanted even thou, I could understand
some case scenario but others I failed to understand, I then watched a video on youtube to get a better understanding of how to get 
the symmetric difference on more than two sets.

## The problem: 
I must Create a function that takes two or more arrays,
that function must return an array of the symmetric difference.

## Symmetric Difference
It is the set of elements which are in either of the sets and not in their intersection. 
So when dealing with more than two sets, you must first find the symmetric difference of the first two and then compare the results to the other set.
## How I approached the problem
## created a variable
I first created a variable which I assigned it to an empty array.
## for-loop
I knew I was dealing with arrays, so I knew that I need to loop through those arrays so I used a for-loop, I was given one parameter
so I knew that the arguments that would be passed will not be one but many so I used arguments
method.In my for-loop, I said loop through my arguments.
I then said my arguments index must be pushed to an empty array.
My empty array now would contain an array of arrays that are passed as arguments.
####    arguments
Arguments object are an array like objects corresponding the arguments passed to a function.
Arguments object are a local variable within a function.
## Created a function
Inside the first function, I created a function that I would use to find the symmetric difference between two arrays.
## created a variable 
I created a variable that I named results that I was going to store my results, I assigned it to an empty array.
#### forEach
Inside my function, I gave it two parameters so that I can be able to compare two arrays.
I then used a forEach method for both the arrays, so that it can go to each and every element in my arrays.
#### if-statement
I nested my forEach statement with an if statement.
Inside my, if statement I used an indexOf method and said that if the second array dot index of the item in my first array
does not exist it should be pushed to an empty.Which means that if a number in my first array is not in the second array then that number must returned.
I then returned that array.
### theory
So the forEach will first go to the first array and compare with the second array when it has filtered out the numbers that do not exist
in both the arrays and store the numbers in the results array. and then it will also go through the second array and compare it with the first array and also filter out the numbers that would not be found in both the arrays and also store them in the results array.
It will iterate until all the arrays are carted for and then will return one array with the results. 
## reduce
In my first function, I then returned my arguments, using the reduce method.
I used my second function in my reduce method.I said return arguments.reduce(mySecondFunction).
## Conclusion
My function was now working, With activity, I learned how to get symmetric difference of more than two sets and how to use a forEach method.
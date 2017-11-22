---
Layout: 
Title: "truthCheck"
date:   2017-11-22 09:40
categories: 
---
## My story
When solving this problem I found it approachable, I had an idea what step I would take to finish the challenge.
This activity required that I check the condition on the given array whether it matches the second argument. 
A truth check value is a value that is considered  true when evaluated in a Boolean context.
All values are truthy unless they are defined as falsy.
## The problem
Check if the predicate (second argument) is truthy on all elements of a collection (first argument).

## My approach
## My rules
Before solving this problem I first wrote down the rules, those rules  were going to help solve my problem.In the rules I include the break-down of the problem.

I need to check the first argument to see whether it contained the key word of the second argument

If the first argument does really contain the item in the second argument ,In  must have a value key in it.
The value key must not be the following values(false, 0, "", null, undefined, and NaN),In order for the truth condition to be met. 

If the value key does not contain the above value a boolean true needs to be retained by my function otherwise if not false has to be retained.

Since we have two arguments that we are comparing against to check for the truth value.

## My first step-for-loop
After writing those rules down it became very easy to think of methods of how I was going to solve the activity.
The problem required that I check the second argument with the first one,I needed to create a for loop in order for me to able to access every element in the first argument.
## My second step-if-statement
After creating my for-loop I could access every element.My main goal was to check if the item in the second argument exist in the first argument and has a value.
My loop was going to go to every element in the first argument,if the keyword is found with no value or not found at all it should return a false, that became a building foundation of my if-statement.
The function is already searching for a truth,So I said that if the condition is not met my for-loop should break and retain the false value(Which means that my index  will go through the first argument the moment it comes across a  falsy  it should just stop and return the boolean false) ,other-wise a true boolean must be returned.
## Conclusion
Write me down the step in this activity really helped me a lot to keep in-track of what the activity really required,my function was now working. 


 
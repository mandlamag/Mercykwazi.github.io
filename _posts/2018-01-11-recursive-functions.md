---
Layout: 
Title:  "Recursive Functions"
date:   2018-01-11 09:40
categories: 
---
# Recursive Functions
# Introduction
I always wonder when I came across code and found that a person has declared a function and along the way that person uses the same function name.
I then came to realization that when that happens they will doing a recursive calling of that function.
A recursive function is a function which either calls itself or is in a potential cycle of function calls. 
## Why use them
These functions are an inefficient means of solving problems in terms of run times.
The function allows  to repeat itself several times, and it gives the results at the end of each iteration.
They  allow you to write efficient programs using a minimal amount of code. 
## Disadvantages
Recursive functions are slower, and takes up more of the stack as well. 
## Example
function factorial(n, accumulator) {
  if (n === 0) {
    return accumulator
  }
  return factorial(n — 1, n * accumulator)
}
factorial(8, 1) 
## Code explanation 
The function above will recursively call the factorial function from 5 to 0 with an accumulator value.
It is important that a recursive function to have a break point otherwise it will lead the function to have an infinity loop.
In this case the  condition n === 0 is the break condition for this function.
# Conclusion
I have realized how useful recursive functions are and also the disadvantages of using one without understanding how they work
    
 

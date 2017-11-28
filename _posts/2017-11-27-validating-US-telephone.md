---
Layout: 
Title: "Validate US Telephone Numbers"
date:   2017-11-27 09:40
categories: 
---
# Validate US Telephone Numbers
## My story
In freeCodeCamp I have just finished my Intermediate Algorithm Scripting,I have just moved to Advanced Algorithm Scripting.
My first exercise is to Validate the US telephone numbers,which I couldn't finish.

## The problem
When-ever the passed string is a valid US phone number the boolean true must be returned.
## My solution
When I saw the problem,I thought of regex because it was given as a hint in the problem.
But as I thought deeper I realized that regex was a little bit complicated than I had though.
I realized that I may know the syntax of it but how I was going to start to approach the problem,
I wasn't sure about it.I knew I had to start somewhere so I took the following steps:
### I created a variable that I would reap my regex in it.
### I knew that the US telephone number contained four digits in it,the order of the digits was 3 at the beginning,
three in the middle and four at the end.When it came to the order of the numbers it was a little bit complicated
because not all the numbers used that order others had a dashes and spaces in between while others didn't have them.
### I only considered the first scenario where the numbers where separated by dashes and their number order was 3,3 and 4 at the end.
### So my regex was in the following order /^\d{3}[-\s]\d{3}[-\s]\d{4}$/ 
The d stands for the digits which are three and in between them there is ether a dash or white-space.
### I then used test() method to validate my string.
The test method would return true if the passed string is indeed a valid US telephone number.
## Conclusion
The written regex only worked for one scenario and the others it did not.My function was not returning what it was expected to return.



---
Layout: 
Title:  "No repeats please "
date:   2018-01-16 09:40
categories: 
---
# No repeats please 
On the the 10th of January I wrote a blog post about how I couldn't solve this problem that I came across on freeCodeCamp.
I took me 6 days to try and solve the problem,I wil share how I manage to solve the problem.
## The problem
The algorithm required the following:
Return the number of total permutations of the provided string that don't have repeated consecutive letters.
Assume that all characters in the provided string are each unique.
## Breaking down the problem
I first had to break down the problem that was given in the following steps:
I first had to find all possible permutations in that given string without having to filter out the repeats.
When I had shown all possible permutations I then knew that I had to filter out the repeated string.
## My approach
After I wrote down my steps I knew my first step was to filter out all permutations so I did the following:
## first function
In the function that we were given on freeCodeCamp it had one parameter which was the string so I decided to use a default parameter,When no value is passed into a function the value of the parameter will be undefined.I did this so that it could be easy for me to use another parameter.
In this function I used heap algorithm sudo code to help me solve the problem.
## Declaring variables
After having two parameters I then declared two variables which one would be an empty  array which i named it c. and the other one was an array I would store my results.
## for-loop
I then had a for-loop which looped through my default parameter.
I then set my c index to zero.
I then closed my for loop and then pushed my a which is the first parameter into my results array.
I then set my index to zero.
## While-loop
I then had a while-loop that said  when index was less than my default parameter.
the following must happen:
## if-statement
I then said as long as my while loop has not broke,inside of the while loop I had an if statement that if c index is less than i (if (c[i] < i) {) then:
##second if-statement
I had another if statement that checked if  index was even (if (i % 2 === 0) {), and if i is even then the following had to happen:
## Splitting the first parameter
I then created a variable that would contain a as a spitted string.
I then declared two more variables,the first one I assigned it to my splitted index zero and the second one I assigned it to splitted index i
## Swapping the variables
One of the steps in the heap algorithm was swapping the two variables which  I just said that my splitted[0] was equal to tempi and splitted[i] was equal to temp0.
I then joined the splitted string.   
## Else-statement
If it happened that index was odd the following would happen:
I  created a variable that would contain a as a spitted string.  
I also declared two more variables,the first one I assigned it to my splitt  c index i and the second one I assigned it to splitt index i
## Swapping the variables
I also swapped the variables which splitt[c[i]] ended up being equal to tempx and splitt index being equal to temp1.
I then joined the splitted string.
I then closed my else statement 
## push
I then pushed my a again into my array.
I then appended my c index by 1,then set i to zero again.
## Else-statement
If it happens that index was greater than my default parameter, c index would be equal to zero and I also appended i by one.

I then closed my  else and while loop.
## All permutations
Now the code above gave me all the permutations that the string passed in would produce,now my following step was to filter out all the repeating  strings.
## My second function
I knew I had to create another function that would filter out all the repetitions in my string.
## filter-method
I  then used the filter method to filter through my results array so that it could remove all the repeating strings.
## regex
In my return statement of the filter function  I used the regex method .match() said that if the letters that are passed do not have more than one word that matches them then they must be returned
I then closed my function.
## My final return
I then returned my results array which was contained  permutations that do not repeat,I then used the .length so that it could give me the length of those permutations.
My function was now working
## Conclusion
Solving this algorithm I learned a lot of things that include being able to read and understand sudo code and also being able to swap variables around,I also learnt more about permutations.
    
          
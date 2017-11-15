---
Layout: 
Title: "Smallest-multiple"
date:   2017-11-14  09:40
categories: 
---
# Smallest Common multiple
## Follow up on the smallest multiple problem that wasn't solved.

## User story
Yesterday I came across a problem in freeCodeCamp but I couldn't finish the problem.

## Requirements of the problem
### It was to find the lowest common multiply of the two given numbers 

### The same multiple has to be evenly divided by both arguments given.

### The multiply should not only be divided by the two arguments but also by all the sequential numbers in the range between those numbers

### The numbers given are not sorted.

# My approach
## sort
I used the sort function to sort every argument from the smallest to the highest as this was also a requirement.
## Declared my variables
I declared 4 variables being:
####### an array which I assigned it to be empty.

####### a variable smallest which I assigned it to be array at index 0
I did this because I knew that what ever argument that is been passed through an array the smallest number will always be the at index 0.

####### a variable highest which I assigned it to be array at index 1
I did this because the two values that are always passed in,the highest  will always be array index 1.

####### a variable multiply which I assigned it to be equal the highest
I did this because In order for one to get to the next multiple he/she must start adding from the last multiple which in this case is the highest number.

## created a validity checker function
Inside my first function I created another function that checked whether the value passed was a valid multiple.
#### for-loop
Inside my validity checker function I had a for-loop

In my for-loop I assigned my index to be equal to the smallest value because that will the the starting point.

I then said that my index my be less or equal to my highest value because I wanted to also include my last value in the range.

I then push my index to an empty array.

Now an array contained all the values that are in the range of the two given numbers.
##### if-statement
Inside my for-loop I  had a conditional statement that said whenever my multiple is dived by the index and the remainder is not zero then a boolean false must be returned.
If other-wise true must be returned.
###### example
given an array of [1,5]
the range of these numbers are[1,2,3,4,5] 
if my multiple is 60 and my index is an the given range numbers, when you divide 60 by the range it leaves zero as a reminder there for my if statement will return true.

## While-loop
After closing my validity checker function I then created a while-loop.
I called my validity function and said that if my conditional  statement is not true then it should increment multiple with highest.
###### example
if my multiple is 5 and my index is 2 ,when you divide 5 by 2 it will  not give you the reminder of zero so my while loop will go and add 5 to my multiple and the 
loop will go on until it finds the correct multiple.

## Return 
I then returned multiple.

# Conclusion
My function was now working.



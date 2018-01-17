---
Layout: 
Title:  "Updating inventory"
date:   2018-01-09 09:40
categories: 
---
# Introduction
Updating inventory system is one of the things that happen in our day to day life.Keeping track the number of inventory you may have is very important to any business.
It also helps to know whether you need to buy stock or you have enough.
## The problem 
We are given two arrays that contain data, One needs to compare the first array which contains the inventory that we currently have with the fresh delivery that has just arrived.
If the items in the first array are also in the second array you need to add both the numbers and return the total with one name.
If other items appear in array 2 and not in the first array they should be added in the first array that will be returned.
When returning an array the items need to be arranged in alphabetical order.
## My approach
Yesterday I could not finish solving this problem because I could not sort the items returned in an alphabetical order.These are the steps I used to solve the problem.
### first-function
I first created a function that removed items that I did not match the item that is in array1.I used the filter method to filter out items that did not match
### second-function
I then had another function that took two arguments the first being the array that contained the inventory that we currently have and the second one being the fresh delivery that needs to be updated.
### for-each
I then used a forEach to loop through every element in my second array.
### for-loop
Inside my forEach, I used a for-loop that looped through the first array 
### if-statement
Inside my for-loop I then said that each and every item that is passed in array2 index 1 is strictly equal to items in array1 index 1, Then the two needed to be added.
I then called my remove function to remove the duplicates.
### second if-statement
The second if statement said that if the items in the second array do not exist in the first item it should be added to the first item.
### sort
Yesterday I could not sort the array because I just used the sort function, but I learned a newer way to combine with the sort function that I was using.
I had to use a conditional statement to my if statement  I said that if a was less than b a negative one must be returned else if a was greater than b then 1 must be returned else zero should be returned.
## Conclusion
My function was now working.The lesson that I learned from this activity was to use an if statement with the sort function and how a forEach really works.
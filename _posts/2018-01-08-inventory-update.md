---
Layout: 
Title:  "inventory update"
date:   2018-01-08 09:40
categories: 
---
# The problem
This is my first blog post for 2018, It is the problem I was solving rather I tried to solve in freeCodeCamp today.
I couldn't finish the problem but I managed to solve part of the problem today.
The activity requested that:
Compare and update the inventory stored in a 2D array against a second 2D array of a fresh delivery.
Update the current existing inventory item quantities (in arr1).
If an item cannot be found, add the new item and quantity into the inventory array
The returned inventory array should be in alphabetical order by item.

# My rules
I first wrote down the steps I was going to follow to solve the problem, In other words, I had to break down every instruction to my own simple understandable manner
These are the rules that I wrote down:
I was going to compare two (2D arrays) against each other the first one being the current inventory and the second one being the new delivery.

After comparing the two arrays I had to update items that were not found in arr1 but are in arr2

# My approach
## first function
I first step was to create a function that will filter out when comparing with two arrays it will filter out the name that appears in both arrays.
## second function
I then created another function that took two arguments which in this case two arrays, which I named them arr1 and arr2.
## forEach
I then used a forEach method to loop inside my second array.
## for-loop
Inside my forEach, I used a for-loop to loop inside my first array.
## if-statement
Inside my for loop I used a conditional statement I said that if index 1 of arr2 is strictly equal to  arr1 index 1 then I said there must add the two together and then called my filter function so that will remove the duplicated name.
## Second if-statement
I then had another if statement that said if items are not found in arr1 but there are there in array2 then they should be pushed to array1.

# Conclusion
At the end of the day my function was adding and replacing what was not there in the other array but it was not sorting out the array in alphabetical order.


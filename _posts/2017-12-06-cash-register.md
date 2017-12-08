---
Layout: 
Title:  "Cash-register"
date:   2017-12-06 09:40
categories: 
---
## The problem
Today in freeCodeCamp I was faced with the tusk of designing a cash register drawer function checkCashRegister()
The function had the following conditions:
If change is less than the cash in register a string "Insufficient funds must be returned"
Return the string "Closed" if cash-in-drawer is equal to the change due.
Otherwise it must return change in coin and bills, sorted in highest to lowest order.

## My approach
When dealing with the problem I had no clue where to start at solving this problem,but I knew that I had a 2 dimensional array so I was forced to either use a for-loop or a reduce method
### Created variables
So I created a variable called change were I said that change was equal to the money that the customer pays with minus the price on the goods/good that the customer is paying.
Then I created another variable that stored all the money register which I called it register.
My last variable was an empty array that stored my change.
### reduce method
I then used a reduce method to try and flatten the 2D array.
Which worked now the value that the reduce was returning was a decimal number.
#### Math-round
To solve the decimal problem I used the Math.round() method  that rounded the money to the nearest number.
## Conclusion
I spent the day accomplished that,I could not solve the problem,But with the progress that I made I'm sure that i will be able to solve it tomorrow.
It took me a lot of time to try and understand what the problem was requiring,The most valuable lesson I leant today was the importance of writing sudo code before going straight to code.

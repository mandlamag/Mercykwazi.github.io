---
Layout: 
Title:  "Building a javaScript calculator "
date:   2018-01-22 09:40
categories: 
---
# Building a javaScript calculator 
My last blog post I mentioned that I was done with the Advanced Algorithm Scripting,my next task in freeCodeCamp,is to build a javaScript calculator.
I found this project a bit challenging but in a good way,I did a part of what the project require.
## The problem
Build a JavaScript Calculator
The calculator had the following user stories to be fulfilled:

Use whichever libraries or APIs you need. Give it your own personal style.

I can add, subtract, multiply and divide two numbers.

I can clear the input field with a clear button.

I can keep chaining mathematical operations together until I hit the equal button, and the calculator will tell me the correct output.
## My approach
## Html
My first approach to this project was to :
## display screen
I first created a display screen and set its default value to zero.The display screen is for displaying the values when you punch them in your calculator.
## buttons
I then created the buttons that will appear on my calculator,Which were numbers 1 to 9 including the operation signs,cancel and back space key.
When creating number,I gave them them a class so that I can be able to style them using css and also gave them a value according to they numbers.
## javascript
In my javaScript code I created different functions that carter for all symbols and numbers in my calculator,I then used a getElementById method and used the id of my screen so that all the numbers and symbols could appear in my screen display.
function addition() {  
var results=document.getElementById("screen");
  results.innerHTML +="+"
}
function cancel() { 
var results=document.getElementById("screen");
  results.innerHTML +=C
}
function zero() { 
var results=document.getElementById("screen");
  results.innerHTML +=0
}

Conclusion
I then used the functions that I called there in my Html as an on-click so that when ever a button is clicked it calls this function.My next step is to be able to add and subtract the numbers so that I could return a correct value,and also be able to style my calculator.
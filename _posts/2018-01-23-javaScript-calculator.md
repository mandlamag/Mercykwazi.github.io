---
Layout: 
Title:  "Building a javaScript calculator "
date:   2018-01-23 09:40
categories: 
---
# Building a javaScript calculator
Yesterday I wrote a blog post on the project that I started doing in freeCodeCamp about javaScript calculator.
Yesterday I had managed to insert buttons on my calculator and I was able to call my functions that I had created on my buttons.
Today I managed to finish off the project,I will share how I managed to have a working calculator.
## The problem
The calculator had the following user stories to be fulfilled:

Use whichever libraries or APIs you need. Give it your own personal style.

I can add, subtract, multiply and divide two numbers.

I can clear the input field with a clear button.

I can keep chaining mathematical operations together until I hit the equal button, and the calculator will tell me the correct output.
## My approach
Like I mentioned in my previous blog post these are the steps I took:
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
I then used the functions that I called there in my Html as an on-click so that when ever a button is clicked it calls this function.
##  eval()
The only thing that was missing in my calculator was for it when you  add to numbers or multiple them they should return an output.
In order for me to achieve this,I used a javaScript method called eval().
This method Evaluate/Execute JavaScript code/expressions.
It became very easy because this method will evaluates or executes an argument.

I used this method in my equal function so that when ever the user press the equal sign it will execute the function.
In the equal function I created a variable that will reap my document.getElementById method,I called the screen id inside my method so that it will be displayed in my screen.
I then used the eval() inside it I put my variable.
function equal() { 
var value=document.getElementById("screen").innerHTML;
  var ans = eval(value);
  document.getElementById("screen").innerHTML= ans;
 
}
# Conclusion
My project was complete and working perfectly fine.
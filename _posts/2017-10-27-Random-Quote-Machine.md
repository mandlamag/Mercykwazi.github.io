---
layout: 
title:  "Building a Random Quote Machine "
date:   2017-10-27 09:40
categories: 
---
Most people enjoy reading inspirational quotes,In order to uplift their spirit.
When we were given the project to build a random quote machine the first thing that came up in my mind was that I wanted to machine to generate inspirational quotes.

Well codePen is divided into 3 sections were you have your Html,Css and your javaScript.
Under the javaScript,I decided to have a variable which i named myQuotes that will contain all my quotes  in an array form that I wanted my machine to generate.In this case i only choose quotes that were inspirational.
I then created a function which I named it quoteGenerator() inside my function I decided to create a variable
named randomNumbers.In my variable I needed to generate a random whole number that ranges from 0 to the length of my  myQuotes array.I used a math.floor method.
I also did this so that when ever a person can click on my random button the quotes might came randomly.
Still inside my function I need a way that will transfer my quotes into the button were the user will be able to access them so I used the document.getElementById()method and I also created an Id in the Html section that will enable the quotes to be displayed in Html.  

In my html I had a div which had an Id  named quoteDisplay,which was used in the  document.getElementById()method in the javaScript section.
I also created Two buttons the first button was were my  user would click in order for him/her her to access the quotes.
The other button purpose was for a person to click and  be able to tweet out the quotes,the button was a tweet button.
Creating the first button I used an on-click  button that very time you click on the button, it will run the function  quoteGenerator(),
When it came to the tweeter button which  had an href  link that every-time you click the tweet button it will direct the user to twitter.

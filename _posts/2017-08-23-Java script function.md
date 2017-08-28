---
layout: 
title:  "Java script function"
date:   2017-08-24 09:40
categories:  
---
It is  a block of code designed to perform a particular task.
It is excecuted  when it is called.
eg 
You have an id called "demo"
function myFunction(s1,s2){
return s1*s2,
}
document.getElementById("demo").innerHTML=myFunction(4,3),
###Conveting a function from fahenhet to celsius
function toCelsius(f){
return (5/9)*(f-32)
}
document.getElementById("demo").innerHTML=toCelsius(77)
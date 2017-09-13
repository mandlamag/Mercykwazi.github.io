---
layout: 
title:  "Javascript-scoping"
date:   2017-09-11 09:40
categories: 
---
Scope is the current context of your code.

You can define your scope global or local.

#####Global scope

It is any variable declared outside of a function.

You can access this variable anyway in your code.

   Example....
<p id="value"></p>
 <script>
 var myVar = "car"
function myFunction(){
  document.getElementById("value").value
  console.log "I love my"+myVar
  </script>

######Local scope
Variables declared within a java script function are local to that function.

Local viriables can only be accessed within that function
Example....
<p id ="value"
<script>
 myFunction()
  document.getElementById("value").value
  console.log "I prefer driving"+myVar
function myFunction(){
  var myVar = "car"
  </script>
 this function will return myVar as undifined because it can not access the code from ouside the function.>

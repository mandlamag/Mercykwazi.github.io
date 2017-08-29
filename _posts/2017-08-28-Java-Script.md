---
layout: 
title:  "java script"
date:   2017-08-28 09:40
categories: 
---
####Iterate over Arrays with map
The map methord is a convenient way to iterate through arrays.
It will iterate through every element of the array,creating new array with values that have modified by the callback function and return it.
It does not modify the orignal array
  ####example 
  var oldArray =[1,2,3,4,5]
  use the map function to add 3 to every value in the oldArray and save the results in the newArray
  var newArray = oldArray.map(function(val){
   return val +3
    })
####Condense arrays with reduce
Reduce is used to iterate through an array and condense it into one value
In order to use it you you pass in a callback whose arguments are accumulator.
An accumulator is the total that the reduce keeps track of after after each oparation.
It has an optional secound argument which can be used to set the initial value of the accumulator.
If no initial value is specified it will be the first array element and will start with the secound array element
  ###example:
  [1,12,5]
  ##when adding
  singleVal=myArray.reduce(function(sum,num){
  return sum+num
  }
   ##when subracting
   singleVal=myArray.reduce(funtion(sum,num){
    return sum-num
    }
###Filter Arrays with filter
It is used to iterate through an array and filter out elements where a given element takes the condition is not true.
It is passed a callback function which takes the current value as an argument.
An array element for which the callback returns true will be kept and an element that returns false will be filered out.
 ##example: Return values less than 6
  var aldArray=[1,3,2,7]
  var newArray=oldArray.filter(function(val)
  return val<6;
  });  
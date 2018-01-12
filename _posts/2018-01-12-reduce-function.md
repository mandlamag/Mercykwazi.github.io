---
Layout: 
Title:  "reduce-function"
date:   2018-01-12 09:40
categories: 
---
# Reduce
One of the most used javascript methods is the reduce method.
It is a method  that applies a function against an accumulator and each element in the array to reduce it to a single value. 
It usually works from left to right.
This method is mostly used when you have two arrays and you want to add the total of both these arrays.
The method takes the following arguments:
## callback
This function is called to execute all the elements in the array.
The callback also takes 4 arguments which are:
#### Initial value
This value is the first value to be executed when a callback is executing,it is therefore important to specify this value because when the value is not specified the first value in the array will became this value,If the array is empty an erro will be returned.
#### currentValue
This the  current element being processed in the array.
#### currentIndex
The index of the current element being processed in the array,this index stars at 0 when it is specified or provided and if not it will starts at index.
#### array
This is an array,which  reduce was called upon.

## Additions
If initialValue is provided in the call to reduce(), then accumulator will be equal to initialValue, and currentValue will be equal to the first value in the array.
example:
If no initialValue is provided, then accumulator will be equal to the first value in the array, and currentValue will be equal to the second.
Example:
var array =[0,1,2,3,4]
 arr.reduce((acc, val) => {
...   return acc + val;
... });
10
The Initial value will start at 0,
but when it is specified like below it will start at 100.
arr.reduce((acc, val) => {
...   return acc + val;
... }, 100);
110
## Conclusion
The reduce function is also useful when you want to flatten a nested array.reduce method works just like a for-loop.



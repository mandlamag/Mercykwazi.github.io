---
layout: 
title:  "find"
date:   2017-09-01 09:40
categories: 
---
The find methord returns the value of the first element in the array that satisfies the provided test function.

If the first element is not found the undifined is returned.

####find index

It returns the index of a found element in the arrau instead of its value.

If you need to find the position of an element or whether to check if the element exist in the array you need to use Array.Prototype.indexof() or Array.prototype.includes()

The find methord executest the callback function one for each index of an array until it finds one were callback returns a value.

If that element is found find immediately returns the value of that element,otherwise undifined is returned.

Callback is invoked for every index of the Array from 0 to length-1 and is invoked for all index not only those who have been assigned values.

Find does not mutate the array on which it is called which means it does not change in form or nature.

The range of elements processed by find is set before the first invocation is set.

If an existing unvesited element of the value at the time that find visite that element index 

Deleted elements are still visited

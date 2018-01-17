---
Layout: 
Title:  "Make a Person  "
date:   2018-01-17 09:40
categories: 
---
# Make a Person
Today in freeCodeCamp I came across an algorithm that I manage to solve.
I will share the whole journey I took to solve this algorithm.
## The problem
I needed to fill in the object constructor with  the given methods below:
    getFirstName()
    getLastName()
    getFullName()
    setFirstName(first)
    setLastName(last)
    setFullName(firstAndLast)
The problem had the following conditions:
Run the tests to see the expected output for each method.

The methods that take an argument must accept only one argument and it has to be a string.

These methods must be the only available means of interacting with the object.
## My approach
I was given a list of methods to use to solve this problem so I used every method that was given to me.
I had an object which was assigned to the given function.
The function had one parameter which had the first and the last name it was called firstAndLast.
## getting the first name and last name
I used the this method() in order for me to be able to access the parameter w that is passed in the object that is outside the outer function.
I then used the parameter of the outer function which contained the firstName and the lastName but it was joined together in a form of one-parameter.
### split
In order for me to be able to access the first name and the last name separate, I needed to split the parameter so that first and last name could be accessible.
I then used used the index[0] method to access the first name and index[1]to access the last name  I then returned the same parameter name.
  this.getLastName =function(){
   var second =firstAndLast.split(" ");
    return second[1];
  };
## getting the fullName
When it came to accessing the fullName,I just returned the given parameter which contained the first and last name already.
## Setting firstName and lastName
When it came to setting a different name from the given one,it was slightly different from getting the name
I created my function still using the this method(),but I added a parameter in the created  function.
Now I needed to re-assign my given parameter from the outer function to the parameter of the function which I just created,I then splitted the given string so that the first and last could be separated,I spitted the string with the index.to set the firstName I used index[1] and for the lastName I used index[0].
Then I returned the variable.
  this.setLastName =function(last){
    firstAndLast =firstAndLast.split(" ")[0] + " " + last;
    return firstAndLast;
  };
## Setting fullName
When setting a fullName,I just said that fullName was equal to the parameter that I had created,I then returned the firstAndLast variable.
My function was now working.
### Conclusion
Solving this problem helped understand objects a little bit better.I also understand  how lexical scoping works

---
Layout: 
Title: "Record Collection"
date:   2017-11-29 09:40
categories: 
---
## Record Collection
When I was attempting this exercise I took a bit of time because I first couldn't understand a few steps but at the end of the day I managed to understand what the problem required.
## The problem
It was to write a function which takes an album's id, a property prop, and a value to modify the data in this collection.
The function must always return the entire collection object.
## Rules
When solving this exercise there were rules that needed to be followed
 - If prop is "tracks" but the album doesn't have a "tracks" property then an empty array must be created,
   before adding the new value to the album's corresponding property.
 - If prop is "tracks" and value isn't empty (" ") then the value must be pushed onto the end of the album's existing tracks array.
 - If value is empty (" ") then the given prop property must be deleted from the album.

With the given rules I was able to then solve the problem because I knew the conditions that I needed to follow.
## steps to solving the problem
I knew I had many conditions that I need to carter for there for I knew that an if statement would be useful
in solving my problem.
I first had a variable named collection that stored all the album's id, a  prop which is made up of an (artist or tracks) and a value.
The first condition I catered for was the one that said if prop has tracks and if the value is not equal to an empty string the value must be pushed to an empty track array.

Inside the if statement I created another if statement that will check if the value is not an empty string if that is the case then no prop and,  will be added to the object. 

An existing key is not updated if the prop already exists.

After closing my two if statements I had an else statement that said that if the value  is an empty string, the prop must be removed from the object.
I then returned my variable collection.

## conclusion
My function was now working properly, returning what was required.



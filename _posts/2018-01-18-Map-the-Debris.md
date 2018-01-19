---
Layout: 
Title:  "Map the Debris"
date:   2018-01-18 09:40
categories: 
---
# Map the Debris
Today in freeCodeCamp,I came an interesting algorithm by the name Map the Debris.It was a bit challenging when it came to solving the problem,but I managed solving the problem.
When it came to this problem it took a lot of research,in order for me to understand what the algorithm required before solving it.
## The problem
Return a new array that transforms the element's average altitude into their orbital periods.

The returned array will have to contain objects in the format {name: 'name', avgAlt: avgAlt}.

The values should be rounded to the nearest whole number.

The body being orbited is Earth.
## My approach
### My research
I first did a research about orbit periods I discovered that, orbital period is the time a given astronomical object takes to complete one orbit around another object, and applies in astronomy usually to planets or asteroids orbiting the Sun, moons orbiting planets, exoplanets orbiting other stars, or binary stars.
After my discovery I knew I had to find a formula that I can use to calculate the orbit period which is T= 2\pi\sqrt{\frac{a^3}{G \left(M_1 + M_2\right)}}
### Sudo
I realized in order for me to be able to solve this I needed to write a sudo code first and see the results before I start to write code,because I realized with with previous algorithm that writing sudo code does help.
### Declaring variable
In the function that was given,they had  two variables that were already declared for me to use.
Which were the GM and the earthRadius.
In the formula which I found we had pi value,So I declared a pie value which I assigned it which a Math.PI()method,because the formula had 2pi so I multiplied pi twice.
I also declared a variable which was an empty array.that I was going to use at a later stage.
My final variable was an a,which I was going to store my calculations at a later stage. 
## for-loop
The function that was given had a single argument that contained an array,inside that array I had an object which had the name and the Average Altitude.
So In order for me to able to access items that were in the array I had to loop through that array with a for loop.
 for (var i = 0; i < arr.length; i++) {}
## adding average and altitude
The formula that I got said that in order for me to get a which is sum of the semi-major axes.I needed to get the sum of the earth radius and average Altitude.
the earthRadius was given but the average altitude was inside the object in an array,so in order for me to get it I used arr index and .average Altitude method.
I then assigned my a variable to the total of earthRadius and average Altitude 
a = earthRadius + arr[i].avgAlt;
## Cubing the total
After I got the value of a the formula said their sum need to be cubed so I used the Math.pow()method.Inside the brackets I inserted the variable a with comma 3 to show that I was cubing it.
## dividing GM
After cubing the total I put it in a variable,and named it cubed and then I divided cubed which GM which was given to me.
## squiring 
As the steps in the formula were progressing the nest step was to square the cubed value,for that one I used the Math.sqrt()method.
## multiplying the pi
The nest step was to multiple pi with the total that I got from squiring.
## Rounding off
One of the rules said the value that is returned my be rounded off.So I used Math.round() method to do that.
## Pushing the objects
After the whole formula steps were complete,I had to push my answer to the object,as the instruction said that an object needed to be returned.
So I pushed to the empty array that I had declared earlier.I pushed arr index to name so that the name will remain the same and created a new name for average altitude I named it  orbitalPeriod and passed in my final answer to it.
Now my function was returning the expected
newArray.push({ name: arr[i].name, orbitalPeriod: finalAnswer });
## Conclusion
The lesson, I lent from this algorithm was how to access objects that are in an array and how to remove another object and replace it with another without using the delete counter.



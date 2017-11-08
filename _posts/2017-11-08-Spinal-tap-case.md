---
Layout: 
Title: "spinalCase"
date:   2017-11-08  09:40
categories: 
---
# Spinal Case
## A follow up on spinal case that I did yesterday and couldn't finish it.

# What was required 

This activity  required that:
If a character on a string is a low-case nothing should be changed from it.
If a character on a string is an upper-case it must be changed to a lower-case.
If there is a white space between the characters on a string the space needs to be replaced with a dash.
If  characters are joined together with an uppercase convert the uppercase into a lower case and put a dash before it,
unless the character is in the begging on the sentence.

# My approach
## first-step:Writing down the rules
This activity made me realize that the reason I did not get it right yesterday was because I jumped into writing the code,
without writing down my rules.
Writing my rules down made it easy for me to plan my approach.
## second step: regex
This activity required for some parts on a string to be replaced,so the first thing I though about was regex
I used the  regex replace method inside the regex I put my lower-case alphabets and upper-case alphabets
together to be replaced with the $1 and $2.
The  $1 being the lower case alphabets and the $2 being the upper-case and I separated the two with the space
,because I want my code every-time there is an uppercase joined together with a lowercase it must be separated by a space.

## third step:toLowerCase
I then used the toLowerCase method to change every letter in the string into lower-case.
## forth step:  replace
After turning every character in my string to  the lower-case, I then used the replace method to replace to replace every
white space and underscore character with a dash.

## Conclusion
When I had done all my step my code was now working.
In this task I realized the importance of writing down steps before approaching my problem.




 



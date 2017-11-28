---
Layout: 
Title: "Validate US Telephone Numbers"
date:   2017-11-28 09:40
categories: 
---
# Validate Us Telephone Numbers
## My story
Yesterday I did not finish this exercise but today I finished it.
## The problem
When-ever the passed string is a valid US phone number the boolean true must be returned.
## My approach
Just like yesterday I still knew that the only way that I was going to solve a problem was using the 
regex method.The only difference would now be that unlike yesterday,I have decided to break my problem into smaller
pieces in this order:
I knew that my test scenario would be based on the following:
 - 555-555-5555 
 - (555)555-5555
 - (555) 555-5555
 - 555 555 5555
 - 5555555555
 - 1 555 555 5555  
 So I decided to use online regex tester and start to test the telephone scenario one by one starting from the less complected one.
 ## first
 I first started with the one with no dashes,I knew that I had to write a regex that will carter for digits that are not more than ten.
 so my regex looked like this \d{10},It was a very simple regex which satisfied my first scenario.
 ## second
 I then moved on to the next one which was still a ten digits number but those digits  had dashes in-between them and they had a pattern in which they were following each
 other they began with 3 digits and then dash and another 3 digits and a dash again then 4 digits.I knew that I needed to add dashes and break the 10 into the sequence in my regex so it looked like this \d{3}[\-]?\d{3}[\-]?\d{4}
 It was still  a simple regex that also coved the first and the second scenario.
## third
The next test scenario was still a ten digit number which was now separated by a space,but still follow the second scenario so I went back to the regex function and said that were there is a dash i also added an escape and put a white space in-between  it \d{3}[\s\-]?\d{3}[\s\-]?\d{4}.
## forth
I then needed to test for a scenario where it began with a bracket notation for the first three digits after the brackets there is no space for the next three digits then a space for the last four digits and the digits were still 10 so I added a bracket in the beginning and an or sign that said the regex can start with a bracket or without it, it should work.(\d{3}\)|\d{3})[\s\-]?\d{3}[\s\-]?\d{4}
## fifth
The next scenario would be a little bit similar to the previous one.The only difference was that there was space after the brackets so the regex still covered this test scenario.
## sixth
I then needed to test for the last part were if the number started with a 1 I then added i with brackets then my function was working



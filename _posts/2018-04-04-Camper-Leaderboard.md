---
layout: 
title:  "Building a Camper Leaderboard
date:   2018-04-04 09:40
categories: 
---
# Building a Camper Leaderboard
Another project that I had to do in freeCodeCamp was to build a camper Leaderboard.
I found this project very interesting because I had use API to retrieve data that I would want in my Leaderboard.
## User stories
As always freeCodeCamp has its own user stories that this project has to satisfy.

I can see a table of the freeCodeCamp campers who've earned the most brownie points in the past 30 days.

I can see how many brownie points they've earned in the past 30 days, and how many they've earned total.

I can toggle between sorting the list by how many brownie points they've earned in the past 30 days and by how many brownie points they've earned total.
Two Apis were provided one being the api for retrieving the scores in all time the other one the scores for recent.

# My approach
In this project as I was going to use an APi I first researched how I would call my api,I used a js library called axios.
## Importing libraries
I first imported the libraries I was going to use in this project I used react and axios I also imported bootstrap for my css styling.I imported everything in my index.js file
## index.js
In this file I had a component which I named Main, it had a render method which returned the class name together with the component which I created called table and an H1 which returned the heading of my project.

## table.js
I had another component which I named it table, because the project specifies that we must return a table that displays the campers who are leading.
In my table class I had a constructor method, I then set the state of two variables into an empty array those variables I would use at a later stage.
  constructor() {
        super();
        this.state = {
            storage: [],
            position: [],
        };
    };
## 1st function
I then had a function which I named recent, In this function I used one of the api to be able to retrieve data of the recent champ leaders.I used the axios to call the api.I then used the setState method to set my storage variable to the data that I got from my api.
### for-loop
I then used a for loop to loop through my response, I then set the state of my position by push the index to position array.
### catch
I also had a catch err function that would just log if there is an err in my code.

 recent() {
        Axios.get("https://fcctop100.herokuapp.com/api/fccusers/top/recent")
            .then(response => {
                this.setState({ storage: response.data });
                for (var i = 1; i < response.data.length; i++) {
                    this.state.position.push(i)
                 
                }
            })
            .catch(err => {
                console.log(err);
            });
    }
## 2nd function
I had a secound function which I called componentDidMount, In this function I used the second api that got the data of the all time winners, I still used the axios library.
I also set the state of my storage with the response I got from the api.
I also had a catch err function.
### for-loop
One of the other requirement of this project was to display the number of the camper so that I can know which position they are sitting on that is why I had the position array. I then looped in that array and set its state by pushing the index but this time I first had to add number in the response because it was not showing.

 componentDidMount() {
        Axios.get('https://fcctop100.herokuapp.com/api/fccusers/top/alltime')
            .then(response => {
                for (var i = 0; i < response.data.length; i++) {
                    response.data[i]["number"] = i + 1;
                    
                }
                this.setState({ storage: response.data });
                console.log(response.data)
            })
            .catch(error => {
                console.log(error)
            });
    }

## render
In my render method I renderd the table, which I created using the thead and the tbody.
### thead
In my thead I displayed the requirements which were the index which was indicated by the # sign,Images,the camperName,the recent scores and the all-time scores.
##### buttons
I made the recent and old time scores in my thead to be buttons I used the onClick method so that the user can be able to click either the buttons to see the type of scores he/she wants to view.
### tbody
In my tbody I need to displayed those items that were in my thead.So I used the map method to map through my data which was stored in my storage variable.
I passed the parameter that was called userData in my map method.
I then used that parameter.to access each and every element in my thead
eg.to access the recent score I would say  <td>{userData.recent}</td>
 
# Conclusion
My project was complete and it was satisfying all the user stories.



                     


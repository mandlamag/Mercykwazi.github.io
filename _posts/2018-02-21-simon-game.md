---
layout: 
title:  "simon-game"
date:   2017-02-21 09:40
categories: 
---
# simon-game
I haven't written a blog post for quite a long time,I have been busy with the freeCodeCamp projects that I have come across.
I will share my journey I took in solving one of the four projects which is the Simon-game.
When It came to solving the simon-game it is one of the projects I came across in freeCodeCamp that I found very interesting.
When I first read the user stories that I need to satisfy,I thought to my self who designs such a game,I did not even have a clue on what or where I was going to start my game,but I was also excited to see the end results of my game.
## The user stories
The challenge that I was solving as I have mentioned was to create a simon game. The simon game had have to satisfy the following user stories:
 I am presented with a random series of button presses.
 Each time I input a series of button presses correctly, I see the same series of button presses but with an additional step.
I hear a sound that corresponds to each button both when the series of button presses plays, and when I personally press a button.
 If I press the wrong button, I am notified that I have done so, and that series of button presses starts again to remind me of the pattern so I can try again.
I can see how many steps are in the current series of button presses.
If I want to restart, I can hit a button to do so, and the game will return to a single step.
I can play in strict mode where if I get a button press wrong, it notifies me that I have done so, and the game restarts at a new random series of button presses.
I can win the game by getting a series of 20 steps correct. I am notified of my victory, then the game starts over.
Hint: Here are mp3s you can use for each button: https://s3.amazonaws.com/freecodecamp/simonSound1.mp3, https://s3.amazonaws.com/freecodecamp/simonSound2.mp3, https://s3.amazonaws.com/freecodecamp/simonSound3.mp3, https://s3.amazonaws.com/freecodecamp/simonSound4.mp3. 
# My approach
I first did a research about how simon game works and after carefully reading the user stories I was able to have a picture on how I was going to solve this game.
## My javaScript 
#### Object
I had an object in that object contained counter,all the possible colors that my game will flash,it had an array that stored the colors that are flushed and an empty array that would record the player selection when ever he plays,it also had different sound clips for each and every colour and it also had the value of strict-mode.
var game = {
        count: 0,
        color: ["white"],
        possibleColors: ["red", "blue", "green", "yellow"],
        gameInProgress: [],
        player: [],
        sound: {
            red: new Audio('https://s3.amazonaws.com/freecodecamp/simonSound1.mp3'),
            blue: new Audio('https://s3.amazonaws.com/freecodecamp/simonSound2.mp3'),
            green: new Audio('https://s3.amazonaws.com/freecodecamp/simonSound3.mp3'),
            yellow: new Audio('https://s3.amazonaws.com/freecodecamp/simonSound4.mp3')
        },
        strict:"Off",
    };

### Add color
I then had a add color function the purpose of this function was to randomly select different colors and add them to the gameInProgress array.
In order for the my function to randomly select the colors, I used the .random() method.I said possible colors.length multiplied by the math.randomly.In this function I then called the flash() function that I will later explain.In order for me to access the items that were inside my object I used the name of the object.what ever I want to access.

### flash()
I then had another function flush the purpose this function was to make colors flush so that the player can know which color to click.
In this function I used the document getElementById method so that I can be able to display my counter,I used the id that I had created in my html and I said that it was equal to the length of my gameInProgress because the length of the colors that will be displayed is equal to the length of the the gameInProgress.
I also had a variable i =0; I also create another variable changer which I equal it to the function of setInterval.
The function setInterval main purpose is to add the class that I declared in my css to the colors that are in the gameInProgress.I declared these class so that when ever the color flashes maybe red the background color should remain dark-red,as this was one of the requirements of the user stories. I set this to last for 1000 milliseconds.
I also had another function setTimeout which would remove the class that I have set after 500 milliseconds.This is so that the player be attentive because if not the wheel will flash and he will not be able to tell which color it was.
I then incremented my i 
I then had a conditional statement that said if if i was strictly equal to the gameInProgress length the interval of my variable should be cleared.
The reason I called this function on add color was that when ever the color is added in an array it should flash the color that it added so that the player can be able to see which color he needs to select.
function flash() {
        document.getElementById("countspace").innerHTML = game.gameInProgress.length;
        var i = 0;
        var change = setInterval(function () {
            console.log(game.gameInProgress[i])

            document.getElementById(game.gameInProgress[i]).classList.add(game.gameInProgress[i] + "_dark")

            setTimeout(function () {
                document.getElementById(game.gameInProgress[i - 1]).classList.remove(game.gameInProgress[i - 1] + "_dark");
            }, 500);
            i++;
            if (i == game.gameInProgress.length) {
                clearInterval(change)
            }
        }, 1000);
    }
#### function startGame() 
I had another function that checked  the length of my gameInProgress and if it finds out that its length is greater than one which means that the game is in progress so if the player can click the start game button again it should alert them that the game is already in progress.
if the game is not in progress it should call the add color function,which means that the player can start the game.
        if (game.gameInProgress.length > 0) {
            alert('sorry, game already in progress');
        } else {
            addColor();
        }
    }
#### function restart() 
The purpose of this function was to enable the user to restart the game if they feel like it,In order for the user to do that both the array that contained the colors that he needs to click and the array that records his patter so I set those array both to empty.I then called the startGame function().
        game.gameInProgress = [];
        game.player = [];
        startGame();

    }

---
layout: 
title:  "Mark-down-Preview
date:   2018-03-29 09:40
categories: 
---
# Mark-down-Preview
I was doing a project in freeCodeCamp which said that I must build a mark down Preview.
Mark-down is defined as a is a lightweight markup language with plain text formatting syntax. 
It is designed so that it can be converted to HTML and many other formats using a tool by the same name
## User stories
Just like the previous project that I have created the mark down Preview had also the user stories that I needed to follow.
User Story: I can type GitHub-flavored Markdown into a text area.
User Story: I can see a preview of the output of my markdown that is updated as I type.

I was also given a package I can use to convert the text into markdown, but the package was not composary if you had a different package you were allowed to use it.

##  importing 
In order to start this project I used a my app file which I imported from the react tutorials
I then imported a library react as this was the labriary I was going to use to create my project.
I also imported the package marked which was recomended by freeCodeCamp in order for it to convert my text to markdown.

## index.js
This was my main file where I imported all the libraries that I was going to use.I had a class which I called a convert  which was going to render the id that I declared in my html.the render method also returned the two other class that I would discuss below witch are Input and markdown.
In my converter class I had a constructor method where I set my input state to an empty string.
I had another function which I called change state,which took and iteam as its parameter, I then set my state using the this.setState method  setting my input to the passed parameter iteam.

## input.js
I then had another class which I called the input.In this class I had  a function called handleChange witch passed in an event.
I also had had a constant witch I named iteam which I assigned it to e.target.value;
I then called in my changeState function. 
  
 handleChange(e) {
        const iteam = e.target.value;
        this.props.changeState(iteam);
    }

### render
In this component in my render function I rendered an text area, I then called an onchange method which I passed in the handleChange method.

 <textarea placeholder="Please type your text here..." onChange={this.handleChange.bind(this)} ></textarea>

## mark.js
In this class I named it markdown.
I first a library called markdown which was going to convert everything that was typed in a text area into a markdown.
In this component I just rendered an html method called dangerouslySetInnerHTML.

# Conclusion
In my index.js in my render method In the Input component I called the changeState method which set my state to iteam,I then bind it with this.
In the Markdown component I created a variable called result,which I assigned it to this.state.input.
My app was up and running
        
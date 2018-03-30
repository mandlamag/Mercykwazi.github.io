---
layout: 
title:  "Document Object Model"
date:   2018-03-27 09:40
categories: 
---

## DOM
In react I often come across with the DOM,So today am writing a blog post explaining what it is and how it used in react.
Just a quick react react is defined as an open source library that is used to develope UI(user Interface).

DOM stands for Document Object Model and it is an abstraction of a structured text.
This text is usually in HTML and it is called the HTMl DOM.
In the DOM html elements become nodes.
DOM is an in-memory representation of html text.
## Issues you can come across in the DOM
### It’s hard to manage. 
It is sometimes to manage the DOM especial when your DOM is made up of thousands of divs,The DOM is said to have a tree structure  so if  you have to tweak an event handler. If you lost the context, you have to dive really deep into the code to even know what’s going on.
This will result in  Both time-consuming and bug-risky. 
#Virtual DOM 
we have this type of DOM which is the Virtual one.
It is an abstraction of the HTML DOM.
It is also a lightweight and detached from the browser-specific implementation details.
It allows React to do its computations within this abstract world and skip the “real” DOM operations, often slow and browser-specific.

var CommentBox = React.createClass({
  render: function() {
    return (
      <div>
        Hello, world! .
      </div>
    );
  }
});
The code below will be rendered in a DOM.
## Conclusion
The DOM is one of the most important element in react because it displays what will be viewed by the User.
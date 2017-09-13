---
layout: 
title:  "An event listiner"
date:   2017-09-04 09:40
categories: 
---
Once set on an applet object, an event lister waits for some action to be performed on it.

That action can be a mouse click, mouse hover,pressing keys,click of buttons.

The class you will be using e.g JButton reports the activity to a class by the class using it.

Then the methord decides how to react,because of that action,usually with seriws of If statements to determine which action it was perfomed on.

#####Example 

Adding an event listener that fires when a user clicks a button

	document.getElementById("myBtn").addEventListener

	("click",display)

######Event handlers

Events can be interactive, they are actions like being clicked,detecting pressed keys.

The on Event handle is usually named according to the event it is designed to react to.

An event handler can also be using propertise on many mon-element objects that generate events.

A handler registered via an on <....> will be available to the corresponding on <...>, but not the other way around.


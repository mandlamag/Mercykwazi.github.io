---
layout: 
title:  "react-life-cycle"
date:   2018-03-26 09:40
categories: 
---
 # React-life-cycle
 A human being has a life-cycle,he is born he grows and dies so does react,It also has its own life-cycle.
 Life cycle is difined as a the series of changes in the life.
 The react life cycle is made up of the following:
The life cyle is divided into three main sections which is the Initializationt, State Changes and the Props changes

# Initialization
### getDefaultProps and getInitialState.
 This phrase of the life cycle is called once, when initially rendering the component.
## getDefaultProps
This stage can be used to define any default props which can be accessed via this.props.
## getInitialState
This stage enables to set the initial state value, that is accessible inside the component via this.state.
## componentWillMount 
This method is called before the render method is executed.
In this phrase state must not be set because when you set state the re-rendering will not be triggered.
## render 
This method returns the needed component markup, which can be a single child component or null or false.
## componentDidMount 
This method is called after the render method, You can access the DOM with this method.

# State Changes
The state will trigger the following methods
## shouldComponentUpdate
It is always called before the render method to check whether a re-rendering is needed or can be skipped.
## componentWillUpdate 
This one is called when shouldComponentUpdate return true.
## componentDidUpdate 
This one is called after the render method.

# Props changes
This method will trigger the following life cycle

## componentWillReceiveProps
It is only called when the props have changed and when this is not an initial rendering

# Unmounting
This method triggers the  componentWillUnmount
## componentWillUnmount
This method  gets called before the component is removed from the DOM

 
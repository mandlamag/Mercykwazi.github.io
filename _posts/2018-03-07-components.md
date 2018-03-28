---
layout: 
title:  "react"
date:   2018-03-07 09:40
categories: 
---
## Introduction
In my last blog post I talked about react and the render method,today I am going to talk about Components

## Components
Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.
components are like JavaScript functions.
 They accept arbitrary inputs (called “props”) and return React elements describing what should appear on the screen.
## Example
function Welcome(props) {
  return <h1>Hello, {props.name}</h1>;
}
The above function is valid React component because it accepts a single “props”  object argument with data and returns a React element.

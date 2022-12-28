---
layout: essay
type: doNotShow
title: "Emerge, Refine, Implement"
date: 2021-04-28
labels:
  - Design Patterns
  - Best Practice
  - Software Engineering
---


## Patterns are Everywhere

And we [see them everywhere](https://en.wikipedia.org/wiki/Apophenia) too. Our pattern recognition as humans helps us understand how the world around us works. If we couldn’t understand patterns, we’d be much worse at guessing, hypothesizing, and reasoning.

## Emergent Patterns

Good software engineers will notice patterns during development. These patterns (if they proved to work well), might be recorded for future reference by the same team or for other teams. There’s usually a good reason why we stumble across patterns or do things in a systematic way: it works. Over time, some good patterns have emerged, been tested, and then refined by other teams into what we call software design patterns. There’s also the reverse: a so-called “anti-pattern”, which should really be called a “bad pattern” because it is still a pattern, just one that shouldn’t be used.

## Imposing Patterns

Finding these good software design patterns and distilling them down into what makes them work takes a lot of time. Luckily for most developers, the work has already been done: the pattern has been shown to work. These patterns can be imposed (or elements of said patterns) into your development process in order to reap the benefits without the years of work of finding the working pattern. But it’s important to understand why the patterns work, and what situation they apply to. Without understanding these two things, you might be using the wrong tool for the job and make things harder for yourself and your team.

## Patterns in GitClubs

In my team’s [GitClubs](https://uhm-gitclubs.github.io/) project, we implemented a few design patterns. This project was built with Meteor, so the design patterns implicit in Meteor and Javascript are present here. These include the following design patterns: prototype, observer, MVC, and front controller. Specific to our project and not implicit to Meteor and JS, we used the singleton design patterns.

#### Meanings
* Prototype - this is used in object oriented languages, instead of creating new objects in a class, we simply clone the original object, this is how all object orientation works in JS
* Observer - This is when the server (the “subject”) will update the users (called “observers”) on any changes in data as they occur, rather than only doing it on a new request. This is what allows Meteor to have reactive data without refreshing pages.
* Model-view-controller (MVC) - This is when the program and its logic are split into three categories
    * The model contains the database usually, and also handles logic.
    * The view is what the user sees and interacts with; the user interface
    * The controller is how the user’s interactions are processed and handled as commands for the other two components.
* Front controller - this is where all requests to the server are handled by one handler. In meteor, this is the router package used (we used react router).
* Singleton - this is when a class is instantiated only once. We used this for our mongo databases/schemas, which were singleton javascript classes. 

# Class 26 reading notes

## What are the building blocks of a React app?

Elements and Components.

## What is the difference between an element and a React component?

Elements are what components are made of. React components are "reusable peices" that we are able to isolate and use as we see fit. React components are like JS functions they do accept inputs (props) and return the react elements that describe what should be appearing on the screen.

## What are some advantages of React’s component based architecture?

Using components makes it easy to reuse these pieces and of course we are able to place  them anywhere we see fit and we think It would work. Also You are able to simplifly what would be a nested hell with the use of components. By nesting components, you can make each peice very easy to reuse,

## What is JSX and why do we use it?

JSX is a syntax extension to javascript. It can be used alongside react to say what the UI should look like. We also use JSX to create React "elements"

## Describe the process of embedding JavaScript expressions in JSX

We can declare any variable (or JS expression) than wrap is in curly braces (this puts us in JSX world).

` const element = <h1>Hello, {name}</h1> `

## Is it safe to embed user input in JSX? Explain

Its is safe to embed user input in JSX. Because by defauly react 'escapes' any values e,bedded in JSX before rendering them. This ensures that you can inject anything that is not explicity written in your app. Everything is rendered as a string.

## Explain what a React Component is to a non-technical friend

A component is a reuseable individual peice that can be placed where ever you need it to be and you can reuse it as you need. 

## Describe mutability and React Components, specifically, how is the UI updated?

immutable means that once you do create an element you cannot change its children or their attributes. The way you update the UI is to create a new element and pass it to the `root.render()` function. This will change what is being displayed. 

## If changes are made to the UI, what does React update?

If changes are made to the UI react will update what element requires it. This helps not create bugs. 

## Note the naming conventions in the Airbnb React/JSX Style Guide. What pattern(s) do you see?

You would use `.jsx` extention on React components, you would use PascalCase for file names, and you use PascalCase for React components and camelCase for their instanes.

## Looking ahead at this module’s course schedule, What do you look forward to learning?

Im interested in learned more about Graphs, especially since we used them in our midterm. Im interested in learning more about them. 

## What are your learning goals after reading and reviewing the class README?

Im interested in learned more about React, and really getting into it alittle more. I feel like its been a life time since we touched on it and Im honestly kind of excited.

## Things I want to know more about

I want to learn more about functional components and how they are better than class components. 
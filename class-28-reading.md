# Class 28

## Name an alternative to the useState Hook

an alternative to `useState`. Takes in a reducer of type `(state, action) => newState`, and returns the current state paired with the `dispatch` method.

## Why might the useReducer Hook be preferable to the useState Hook?

`useReducer` is prefered to `useState` when you have complex state logic that involves multiple sub-values OR when the new state depends on the the previous state. This also allows you to "optimize performance for components..." that can trigger deep updates since you able to pass `dispatch` down instead of callbacks.

## What are two ways to set the initial state?

You can set the initial state as a second arguement.

`const [state, dispatch] = useReducer(reducer{count:intialCount});`
You can do it the "lazy way" which is ehrn you pass an `init` function as the third argument. `init(initalArg)`

This is lets you extract the logic for calculating the initiL stte outside of the reducer function. This is also helpful for when you have to reset the state later based on a certain action.

## In terms of state, what does useReducer expect to receive as a parameter?

useReducer takes in the the `reducer` function and the current state

## What does useReducer return?

`useReducer` returns an array that holds the current value of the state and a `dispatch` function which allows you to later pass an action and a function.

## Explain dispatch to a non-technical recruiter

Being able to "dispatch" is being able to "send" a set of instructions / action. This has to be carried along a reducer. A reducer is an action that requires two things (the state as it stands, and how we are changing the current state).

## What are your learning goals after reading and reviewing the class README?

Based off of the reading, I am interested in learned more about reducers.

# Class 37 Reading

## Why create multiple reducers?

we are able to trigger changes in one reducer that can effect many reducers which then come together to update the new state object.

## How would you combine multiple reducers?

you would take in your two reducers and combine them within a `combineReducers({})` function
`nameReducer=(state=[], action)=>
 tweetReducer=(state=[], action)=>
 combineReducers({
    name:nameReducer
    tweet:tweetReducer })
``

## How will you manage state as an immutable object? why?

we are able to use change the state by making a copy (spread operater) and attach out new state to that copy.

## combineReducers is a utility function to simplify the most common use case when writing ________

Redux Reducers.

## Explain how combineReducers assembles the new state tree

`combineReducers` calls each slice `slice` and where it stands in its current state and its current action, this gives the slice reducer a chance to respond and/or update if needed.

## How would you define initial state in an app using combineReducers?

 -`createStore`  can take `preloadState` as a second argument, this is used to initial state that was "previously persisted" (like the browsers local storage).

- `combineReducers` take in an object full of slice reducers which creates a function that effects the state that matches with the same key.

## Why will you want to split your reducing functions as your app becomes more complex?

the more your app grows and the more state you have throughout the tree, you will want to split your reducing function into seperate functions, which would manage independent parts of state.

## The _____ helper function turns an object whose values are different reducing functions into a single reducing function you can pass to ____

`combineReducers` `createStore`

## What is a popular convention when naming reducers?

It is a popular convention to name the reducers after the state slice that they manage.
`combineReducers({ counter, todos })`
`combineReducers({ counter: counter, todos: todos })`

# Class 36 reading notes

## What is the first principle of Redux?

To represent the whole state of the whole app as an imutable object, therefore every change that is made in your app is contained in a single object.

## what is a store and what do we use our reducers for within that store?

we have a state tree that is read-only we cannot change the state. We dispatch an action that we use represent the minimal change to the state object. The way we dispatch an item is specify to the reducer what and how this dispatch is updating the state

## Name three Redux store methods given to us by createStore and describe their use

getState() it retrieves the current state of the redux store.
dispatch() lets us dispatch actions to change the state of our app.
subscribe() it lets us register a call back every time an action gets dispatched to update the when we change our state.

## Explain to a non-technical recruiter what combineReducers() does and why it is useful

`combineReducers()` allows us manage our applications state across the board. We use reducers to manage state for different parts of our app. `combineReducers()` allows us to combine all the reducers  so we an manage our global state in one place.
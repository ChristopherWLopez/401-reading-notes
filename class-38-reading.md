# Class 38 Reading

## Why use Redux middleware?

Redux Middleware allows us to write logic that has side effects.
We are able to `do anything` with with our dispatch action. This means that we can make an async call that would create a side effect. Our middle ware also allows us to send things that arent plain action objects as long as our middleware can accept the value.

We area alse able to use such methods like `dispatch` and `getState` This free's is up to make api calls that will effect our state with an asyn function.

## Consider the Redux Async Data Flow Diagram. Describe the flow in your own words

So we start at the UI where we have our buttons that would allows is to dispatch a function to our middleware, this middleware adds a small detour by making an API call of some sort, when this API call gets returned we area then able to finish our dipatch that creates a new state and then we update the slice that is being effected inside of our store.

## How are we accommodating async in our Redux app?

We are using `Thunk` which is an "async function middleware". This middleware allows us to use write our own functions can use `dispatch` and `getState` as arguments.. These function can hold any async logic we want and allows us complete the cycle where our dispatch is able to update the state.

## Why would you need redux-thunk middleware?

`Thunk` allows us to write functions that can hold async logic within it and that function can interact with our redux stores built in methods (`dispatch` and `getState`).

## Redux Thunk middleware allows you to write action creators that return a ____ instead of an action

`Function` This allows you to pospone (async) the dispatch action or it will be dispatched if a condition is met.

## Describe how any return value from the inner thunk function will be made available

we create a "thunk action creator" that is used to create thunk functions. this function can have some arguments. This function returns a new thunk function that takes `dispatch` and `getState` as arguments. We then are able to dispatch the return of that function.

## I want to know more about this ^^


# Class 39 reading

## What concerns are addressed by Redux Toolkit?

RTK set out to address  the big isssues that configuring a store while using Redux was very complicated, there was too many packages to install when you wanted to do anything really useful, and the amount of boilerplate code was alittle overkill.

## What does configureStore() do?

This wraps the `createStore` method to aid in the process of configuration options as well as defaults. This also can add middleware (which ever you supply), you are able to combine reducers, and adds `redux-thunk` by default.  

## How would I use createSlice()?

`createSlice` takes in a single configuration object param, with a name, intialState, and  an object of "case reducers". This function generations action acreator and action types that are tied to the reducers and the state.

## What is Mobx?

`MobX` is a straighforward state management library that is scalable. This is a standalone library but can be used alongside React.

## How does MobX make it “impossible” to produce an inconsistent state?

`MobX` makes state management "easy" by making sure that "Make sure that everything that can be derived from the application state, will be derived. Automatically."

## How would we build a reactive user interface?

We use a Wrapper, the components that are wrapped in this `autorun` keeps said components in sync with the state. This ensures that each component rerenders and without the use of `useState` and all those other setters, that we would have to go through our code base to ensure everything has that specific method. We now just wrap those suckers.

## What take-away(s) did this tutorial provide?

I chose to review the quick-start guide. It was pretty rad to see how simplified everything was made. How we configrue our store, then wrap our affected components with a provider, assuring that those components have access to that store. Next we fill our store with slices, the slices require very simple information : name, initial state, and a reducer which states how the `state` will be updated when we run a reducer. Next we add our slicer to the store by using `configureStore` and within our reducer property we place our reducer inside of it.

# Class 32 reading notes

## How do useReducer and useContext work together to simplify state management in a React application? (At least two paragraphs of prose.)

We are able to combine two hooks inorder to simplify managing state that take several effect handlers by using `useReducer` this makes managing state a bit easier and much more consice. This is very helpful on its own. `useReducer` allows us to really scale back our code that would be required to set state within a certain component. On its own we would have to not only use alot of said event handlers, but we would also have use props (prop drilling) if we wanted to pass this ability down a few component levels... However we can combine two usful hooks.

We are able to combine this simplified state management with the ability to make this state accessibile to any child of said component by using the `context API`. By doing so we are not just minimizing the amount of event handlers and how it pertains a specific `state` (`use reducer`) we are able to make it accessibile by using the `useContext`.

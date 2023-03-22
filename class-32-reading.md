# Class 32 reading notes

## How do useReducer and useContext work together to simplify state management in a React application? (At least two paragraphs of prose.)

We are able to combine two hooks inorder to simplify managing state that take several effect handlers by using `useReducer` this makes managing state a bit easier and much more consice. This is very helpful on its own.

We are able to combine this simplified state management with the ability to make this state accessibile to any child of said component by using the `context API`. By doing so we are not just minimizing the amount of event handlers and how it pertains a specific `state` (`use reducer`) we are able to make it accessibile by using the `useContext`.
